Command Line Options.

These are for advanced users only.  Use at own risk.

Options are read from both the EDDiscovery command line and from an options file.  

The default options file is read from the file options.txt located in the application install folder of EDDiscovery.  To change to another location and file use -optionsfile <filename> on the command line. If just a file name, it will be searched for in the install folder of EDDiscovery.  If a full path, use the full path location.

Options are case insensitive.

Command line options are as follows:

# USER

* -NRW or -NoRepositionWindow : Use default window positions, don't load at previous positions.  Same as holding down shift during program start.

* -Portable : Store EDDiscovery data files in same folder as executable.  If you use this, the EDDiscovery folder must be user writable.

# Advanced User

* -Appfolder : Use this folder instead of EDDiscovery in the <users>/appdata/local folder.  This can be used to separate the data bases of different commanders if required.  Not needed for multi commander use.  Mostly its for debug purposes.

* -Userdbpath: Use this path for the user data base instead of the default appfolder/EDDUser.sqlite file.

* -Systemsdbpath: Use this path for the systems data base instead of the default appfolder/EDDSystem.sqlite file.

* -Olddbpath: Use this path for the old ED Discovery data base (pre 2.2) instead of the default appfolder/EDDSystem.sqlite file. (8.0+ removes the ability to read this DB).

* -Tracelog : Do a tracelog even when debugging.

* -LogExceptions: Log exceptions

* -notheme :  Starts EDDiscovery with default theme  (EDD 8.2.1+) 

Other internal options are present for developer use only.