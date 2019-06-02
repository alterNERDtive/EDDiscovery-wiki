Command Line Options.

These are for advanced users only.  Use at own risk.

Options are read from both the EDDiscovery command line and from:
* Any option file included by the -optionfile <file> option given on the command line.  It will check in both the application install folder and the application data folder for this file if its just a file name.  If its a full path it will read it from that path.
* options.txt if present and located in the same folder as the application install folder of EDDiscovery.exe
* options.txt if present and located in the application data folder (default `%LOCALAPPDATA%\EDDiscovery`)
* dboptions.txt if present and located in the application data folder - this is written by the program if you've moved the databases, so the user should not normally update this file.

Options are case insensitive.  In option files, don't include the '-' character in front of the option.

Command line options are as follows:

# USER

* `-Commander <name>` (11.0+)

Switch to commander <name>.  Use quotes if name has spaces.

* `-NRW` or `-NoRepositionWindow`

  Use default window positions, don't load at previous positions.  Safe mode (hold down shift as you run the program) allows this to be set by the user via a dialog.

* `-NoTheme`

  Don't load the theme.  Safe mode allows this to be set by the user via a dialog.

* `-Portable`

  Store EDDiscovery data files in a sub folder of the executable.  If you use this, the EDDiscovery application folder must be user writable.

# Advanced User

* `-Appfolder <name/path>`

  Use this folder instead of `%LOCALAPPDATA%\EDDiscovery` (where `%LOCALAPPDATA%` is usually `C:\Users\%USERNAME%\AppData\Local`) for the application data folder.

  If a directory name only is supplied, it is stored in `%LOCALAPPDATA%\<name>`.  If a full path is given, it is stored there.

  Ignored if -Portable is given.

  This is useful for debug use, to start a clean ED session while keeping your old data.

  Not needed for multi commander use.

  Example: `-Appfolder data1`

* `-Userdbpath <folder path>`

  Use this path for the user data base instead of the default application data folder.

  This allows the db to be stored somewhere else that the application data folder.  Useful if your SSD is small.

  Note dboptions.txt uses this as part of the safe mode system to move databases around.

* `-Systemsdbpath <folder path>`

  Use this path for the systems data base instead of the default application data folder.

  Note dboptions.txt uses this as part of the safe mode system to move databases around.

* `-Tracelog`

  Do a tracelog even when debugging.

* `-LogExceptions`

  Log exceptions

Other internal options are present for developer use only.
