10.2 adds in support for multiple languages

# How It works

To define a language, a languagename-isotwocharname.tlf file needs to be present either in the .exe folder where EDD is run from (the installer puts these files in there) or in the appdata/eddiscovery/translator folder.

The TLF file defines language strings for all EDD panels, forms, program features etc.

The TLF must be in UCS-BOM-8 format.  Use only notepad++ or visual studio to edit it.

The TLF file may use Include filename to include another file (usually called TLP files)

# Structure in the EDD Solution (Visual Studio)

Check out the code in GIT and use visual studio to edit the main SLN file.

In Eddiscovery project, the VS subfolder Translations contains the source controlled TLF files.  

In Eddiscovery project, the [UserControls subfolder](https://github.com/EDDiscovery/EDDiscovery/tree/master/EDDiscovery/UserControls) contains TLP files containing definitions for the User controls (Panels)

In EliteDangerous project, the [EliteDangerous subfolder](https://github.com/EDDiscovery/EDDiscovery/tree/master/EliteDangerous/EliteDangerous) contains TLP files containing definitions for the Materials and other common ED terms.

In EliteDangerous project, the [JournalEvents subfolder](https://github.com/EDDiscovery/EDDiscovery/tree/master/EliteDangerous/JournalEvents) contains TLP files containing definitions for the Journal event names and formatting strings for each event.




