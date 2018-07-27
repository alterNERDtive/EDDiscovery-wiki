10.2 adds in support for multiple languages

# How It works

To define a language, a languagename-isotwocharname.tlf file needs to be present either in the .exe folder where EDD is run from (the installer puts these files in there) or in the appdata/eddiscovery/translator folder.

The TLF file defines language strings for all EDD panels, forms, program features etc.

The TLF must be in UCS-BOM-8 format.  Use only notepad++ or visual studio to edit it.

The TLF file may use Include filename to include another file (usually called TLP files)

An example-ex.TLF file is kept to show all the IDs.

# Format of the TLF/TLP files

Each line of the TLF/TLP is either a comment (//), blank line, Include statement or a definition.

The format of a definition is:

ID : "english text example" => "Foreign text"
or
ID : "english text example" @

ID is case sensitive and is generally in the form Module.Part.  The shortform .Part is also used which just means, assign it the previous stated module.

The English part after the colon is a guide for what you should be replacing.  Its not actually used in the program. It could be blank ("") for instance and EDD would ok: Warning: "" => "Warnung"

The first form fully replaces the english text in the program with the foreign text - this is the end game!

The second is used during development. It means:
* Debug mode : repeat the program English phrase but with '' around it to show on screen the ID has been recognised.
* Release mode : repeat in program English exactly.  This means that you don't want to translate this section and are happy for it to be in English.

You don't need to translate every bit at once, you can do it as you see fit, and try it between goes.

Beware of the format strings such as .CAPIF: "Companion API failed: {0}" @ These are c# format string, the {N} is replaced by the actual data. 

Keep the {0} somewhere in your translation.  It does not have to be in the same position. You would do: .CAPIF: "" => "Translation make sure you put {0} somewhere"

There are also format strings like: JournalEntry.Fuel: "Fuel:; tons;0.0" @

These need to be keep in the field builder format, the format is Prefixtext;postfixtext;Formatspecifier
JournalEntry.Fuel: "" => "Fuel translated:; tonage translated;0.0"



# Structure in the EDD Solution (Visual Studio)

Check out the code in GIT and use visual studio to edit the main SLN file.

In Eddiscovery project, the VS subfolder Translations contains the source controlled TLF files.  

In Eddiscovery project, the [UserControls subfolder](https://github.com/EDDiscovery/EDDiscovery/tree/master/EDDiscovery/UserControls) contains TLP files containing definitions for the User controls (Panels)

In EliteDangerous project, the [EliteDangerous subfolder](https://github.com/EDDiscovery/EDDiscovery/tree/master/EliteDangerous/EliteDangerous) contains TLP files containing definitions for the Materials and other common ED terms.

In EliteDangerous project, the [JournalEvents subfolder](https://github.com/EDDiscovery/EDDiscovery/tree/master/EliteDangerous/JournalEvents) contains TLP files containing definitions for the Journal event names and formatting strings for each event.

# Debugging it
To use the VS Project translation files directly from the project, define in the EDDiscovery project options -translationfolder folder 2

folder should be the location of the EDDiscovery project translation folder on your disk.  Mine is at c:\code\eddiscovery\eddiscovery\translations

This allows the translator to find the projects translation files directly from your VS project and to search for the TLP parts.  

When distributed, the .TLF and .TLP files will all be in the same folder as the .EXE and thus won't need to be found using a tree search.  Thus you don't need the option.

You could also copy all the TLF/TLPs to appdata/eddiscovery/translation folder, but then you'd have two copies.

In debug mode, the translation system writes to appdata/eddiscovery/translator-ids.txt.  This indicates what files it reads and importantly tells you if any IDs are missing from the translation files.  Use this mechanism when developing new code.

Netlogentry also has a translator scanner which reads the C# source code files and finds any .Tx statements in there.  This is also the other primary way of finding new IDs to add to the translation files during development.



