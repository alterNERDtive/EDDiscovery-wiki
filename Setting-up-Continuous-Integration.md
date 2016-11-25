# Setting up AppVeyor

* Go to https://github.com/integrations/appveyor
* Click `Add to GitHub`
* Under the permissions and Organization access, click `Authorize application`
* After authorizing the application, in AppVeyor click `+ New Project`
* Select `Public repositories only` and click `Authorize GitHub`
* Review the permissions and click `Authorize application`
* Under the appropriate organisation or your username, mouse over the project (`EDDiscovery`) and click `+ Add`
* AppVeyor should now automatically build every new commit or pull request, and save a portable version of the build as an artifact.

## Getting AppVeyor build badge

* Click `Settings`
* Click `Badges`
* Copy the markup from `Branch sample markdown code` under the `master branch status badge`
* Paste it wherever the AppVeyor status should be displayed

# Setting up Travis-CI

* Go to https://github.com/integrations/travis-ci
* Click `Add to GitHub`
* If necessary, click `Grant access` next to the appropriate organisation
* Under the permissions and Organization access, click `Authorize application`
* After authorizing the application, in Travis, under `My Repositories` click the project (e.g. `EDDiscovery/EDDiscovery`)
* Click `Activate repository`
* Travis-CI should now build all new commits and pull requests, and provide a build status for any pull requests

## Travis CI build badge

* The URL to the build badge is based on the GitHub repository path - e.g. the Travis-CI build badge image URL for `EDDiscovery/EDDiscovery` is `https://travis-ci.org/EDDiscovery/EDDiscovery.svg?branch=master`
* The build badge markup should be: `[![travis](https://travis-ci.org/EDDiscovery/EDDiscovery.svg?branch=master)](https://travis-ci.org/EDDiscovery/EDDiscovery)` - copy and paste that where the AppVeyor build badge should be displayed.
