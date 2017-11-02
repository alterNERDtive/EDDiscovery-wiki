# Interaction with Elite Dangerous

Elite Dangerous creates journal files, with journal entries, in a folder as it runs. It places those files in c:\users\ _username_ \Saved Games\Frontier Developments\Elite Dangerous.

EDDiscovery reads those files, and uses that as its information source.

See the [[settings panel|Using the Settings Panel]] for the ability to read journal files from places other than this default folder.

# Journal Entries

There are over 100 types of entry, containing data about your ED game.  Most of the data the user needs is in these entries.

# Commander Creation

When EDDiscovery reads the journal files, if it sees a new commander listed in the journals, it will search the commander table in [[settings|Using the Settings Panel]] for an existing commander.  If does not find a commander of the name given in the journal, it will create a new entry in this table for the commander. 

If your using EDDiscovery for the first time, then the first new commander found becomes your commander and is selected on the [[History Tab|Using the History Tab]] Cmdr entry. 

If you already have a commander, the current commander chosen is not changed.

The journal entries in the file are then associated with a commander. You won't see them unless you've selected that commander. Use the [[settings panel|Using the Settings Panel]] to see which commanders you have. Use the toolbar commander selection at the top to change the commander.

# Reading old pre 2.2 log files.

If you had verbose logging on and have old netlogs, you can still read them in.  See [[menu options|Menu Options]].  If you did not have verbose logging on (and you will remember if you did!) then your out of luck.  The previous netlogs had only jump information in them.
