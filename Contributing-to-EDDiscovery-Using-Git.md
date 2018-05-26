The best way to contribute to EDDiscovery is to create a fork of the main project, make changes in your local fork and push them back up as Pull Requests using git.

Figuring out Git can be a bit of a challenge to those more familiar with traditional server side SCMs like Subversion. It's probably easiest to try and forget everything you know, start again and work through a good tutorial or screencast. One such example is:

http://gitimmersion.com/

A lot of the trickier things you will need to do are commonplace, so here is a cookbook on solving this little problems.

# Git Cookbook

I'm also going to give instructions on using the command line tool [Git Bash](https://git-scm.com/downloads). There are other ways to use Git, but it'll be easier to explain it this way.

I'm going to use https repo urls, but ssh works even better if you have the public key/private key thing set up right.

Most of these examples assume you have a remote to the main repo called "**upstream**" The initial recipe explains how to create the upstream remote.

#### Recipes:

* [Getting pull request capable for the first time](#getting-pull-request-capable-for-the-first-time)
* [Resyncing with EDDiscovery/EDDiscovery repo](#resyncing-with-eddiscoveryeddiscovery-repo)
* [Pull requests](#pull-requests)
* [Going nuclear: Resetting the master branch](#going-nuclear-resetting-the-master-branch)

### Getting pull request capable for the first time

For all this recipe we're going to pretend to use a fictional github account called **YOUR_GITHUB_NAME_HERE**. Substitute that username for your own.

* Go to Finwen's EDDiscovery page. Make your own fork. Do this from here: 

https://github.com/EDDiscovery/EDDiscovery

* Go to your clone repo page: 

https://github.com/YOUR_GITHUB_NAME_HERE/EDDiscovery

* Clone your forked repo from Git Bash. Create an upstream remote to the main remote repo

```
$ git clone https://github.com/YOUR_GITHUB_NAME_HERE/EDDiscovery.git
$ cd EDDiscovery
$ git remote add upstream https://github.com/EDDiscovery/EDDiscovery.git
```

* You now have an 'upstream' remote for syncing with Finwen's original repo and an 'origin' remote for your github fork. Check that:
```
$ git remote -v
```

* Create a feature branch and checkout onto it using `git checkout -b`:
```
$ git branch
* master

$ git checkout -b add-red-button
Switched to a new branch 'add-red-button'

$git branch
* add-red-button
  master
```
This step is important because now when you make a pull request the branch name will be used. If at any point you want to make a quick pull request for a bug fix you will need to checkout master, pull down the latest from upstream, create a new branch and manage that pull request completely separately. No leakage between feature branches that way!

Off you go. Build something beautiful!

### Resyncing with EDDiscovery/EDDiscovery repo

Ok, you probably already know how to pull down the latest from a remote repo. It's normally something like this for master branch:

```
$ git pull origin master
```

Or if you really know what you're doing you'll do this to avoid merge bubbles:

```
$ git fetch
$ git rebase origin/master
```

But this won't do you any good for contributing to EDDiscovery because all the change is happening on Finwen's remote repo, not your forked copy! So how do we get our stuff all synced up?

First off lets update our local master with the upstream master

```
$ git checkout master
$ git status
```

Confirm that you don't have any uncommitted files. If you do commit them, stash the, move them out of the way, whatever.

```
$ git fetch upstream
$ git rebase upstream/master
```

This will update your local copy of "remote branches" from Finwen's upstream repo and then modify your local commit history to incorporate upstream commits. If you run into conflicts you will need to work through an "[interactive rebase](https://help.github.com/articles/resolving-merge-conflicts-after-a-git-rebase/)" to resolve them. Read up on it then work through them.

When you're done you check your new history with these commands:
```
$ git log
$ git log -p     <-- shows commits as well as commits
```
The latter version shows the diffs. you might want to search those diffs for "====" to make sure you didn't miss a conflict.

Now you can go ahead update your own repo

```
$ git fetch origin
$ git rebase origin/master
$ git push origin master
```

... which should push your changes up. You can check this by looking at sources from the github site. 

You will probably need a "force" push if you had to merge anything. Because the commit history has been modified:

```
$ git push -f origin master            <-- -f makes it a force push master Skywalker.
```

Force push is a dangerous tool, but you're only using it on your own fork, so it's safe enough.

Finally you probably have a local feature branch which needs to be updated with remote changes in the upstream repo; this was probably why you had to sync up in the first place. Basically do the same thing you did for the master branch but now with your feature branch:

```
$ git fetch upstream
$ git branch my-newer-purple-button
$ git checkout my-newer-purple-button-feature
$ git branch backup-branch-restore-point-case-something-goes-wrong      <--- Optional trick ;)
$ git rebase upstream/master
```

Now's probably a good time to update your remote forked repo on github:

```
$ git push origin my-newer-purple-button-feature
```

Notice I threw in a step for creating a 2nd branch in cause you make a mess of the rebase and want to get back to where you left off.

### Pull requests

Before attempting a pull request you'll want to [pull the latest from EDDiscovery/EDDiscovery](#resyncing-with-eddiscoveryeddiscovery-repo) into your branch by fetching and rebasing. As explained in the previous section. If you don't you may find you have merge conflicts and pain will result.

Done that? The rest is pretty straightforward.

If you're still on master branch you'll want change to a named branch first. If you don't any other work you do may contaminate your pull request. 

You can still fix that by doing this if you have to:

```
$ git branch
* master

$ git checkout -b let-make-the-fonts-all-comic-sans
Switched to a new branch 'let-make-the-fonts-all-comic-sans'
```

Next, push up your local branch to your fork using your fork's remote.

```
$ git fetch
$ git rebase origin/let-make-the-fonts-all-comic-sans     <-- Don't need to do this if you this is your first push
$ git push origin let-make-the-fonts-all-comic-sans
```

Finally view the github web page for you repo fork and click on the green "Compare and Pull Request" button. Before submitting your pull request to make sure the commits listed are your change and only that. Make sure you don't have any leakage from other people or other feature branches! 

### Going nuclear: Resetting the master branch

Ever get into a real mess and want to start again with your repo? Well you could delete your fork in github, reclone and start again from scratch. But that's maybe a little too drastic. How about we try something else? Let's look at ways to get the master branch back to normal. then you can branch off that and get back to normal.

#### Option 1: My master branch is at the wrong commit.

So somehow your master branch is pointing at the wrong thing. you can just move it to the correct place if you can find the right sha (commit code) or another branch that is in the right place. So you just need to find where that is.

Here's 4 ways you can track down your errant commit point:

**1) Make it the same as the fork's master on github**

You just want your local master to be the same as your github fork's master? This should do it:

```
$ git fetch
$ git reset --hard origin/master
```


**2) The logs** (the --all part makes it show ALL commits in the repo)

```
$ git log --all --graph
```

**3) Using a GUI graph view like gitk or Git for Windows**

```
gitk --all
```

Note: Your current HEAD node is a yellow dot. It'll also show there the remote branches are at.

**4) Look in the "reflog" this is a log of all commits ever** (even ones that are 'deleted'):

```
$ git reflog
```

Note the SHA codes are shorter here. Just 7 chars. Doesn't matter.

Found your SHA? Now you just need to change which commit your HEAD is at:

So if I found the latest SHA is supposed to be `25437cf`. Here's how I get my HEAD for master to this point.

```
$ git checkout master
$ git reset --hard 25437cf
$ git log
```

See? You're back in the game.

If your have problems pushing your change up to your github fork afterwards you can force it to write to match your local version. It's a little drastic, but you can do this:

```
$ git -f push origin/master
```

Now check on github. The commit history should be the same.

#### Option 2: Blow away my local master and recreate it

First get rid of it:

```
$ git checkout another-branch
$ git branch -D master
```

Did you wave goodbye?

Next what do you want your master to be based off? upstream/master? origin/master? I'm guessing upstream/master so you're back to how the latest build of EDDiscovery is.

```
$ git fetch upstream
$ git checkout upstream/master       <-- Checkout a remote branch
$ git checkout -b master
$ git log
```

Done!

Now if you were working on something before hand you may want to rebase that off of upstream/master too.