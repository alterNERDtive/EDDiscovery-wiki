# Interaction with Elite Dangerous

Elite Dangerous creates journal files, with journal entries, in a folder as it runs.  EDDiscovery reads those files, and uses that as its information source.

EDDiscovery reads journal files by default from c:\users\<username>\Saved Games\Frontier Developments\Elite Dangerous.  This is where ED 2.2 and on place the journal Log files. 

See the [settings page](Using the Settings Page) for the ability to read journal files from places other than this default folder.

# Journal Entries

There are over 100 types of entry, containing data about your ED game.  Most of the data we want is there, some of it is not listed (such as total material/commodity counts) so some of the limitations of EDDiscovery is due to this.

# Commander Creation

When EDDiscovery reads the journal files, if it sees a new commander listed in the journals, it will search the commander table in [settings](Using the Settings Page) for an existing commander.  If does not find a commander of the name given in the journal, it will create a new entry in this table for the commander. 

If your using EDDiscovery for the first time, then the first new commander found becomes your commander and is selected on the [History Page](Using the History Page) Cmdr entry. 

If you already have a commander, the current commander chosen is not changed.

The journal entries in the file are then associated with a commander. You won't see them unless you've selected that commander. Use the settings page to see which commanders you have.

# Reading old pre 2.2 log files.

If you had verbose logging on and have old netlogs, you can still read them in.  See [menu options](Menu Options).
