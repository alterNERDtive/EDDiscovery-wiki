From 10.2, EDD supports multiple languages for its user interface.  You can change the language in Settings.

Language translations are provided by the EDD user community.

Not all sections of the program may have all items translated.  There are a very large number of items to translate so it may be that the author of the translation only concentrated on the primary parts.

## Your language not there? Translation not complete?

Then contribute!

Language translation files are simple.  They are found inside (for the release version) the .exe folder (c:\program files\eddiscovery\eddiscovery normally). 

The primary translation for a language is called a .tlf file, and is named languagename-iso 2 or 3 char code.tlf.  For instance italiano-it.tlf.  Any language files found in the .exe folder using the .tlf and this format name will be presented in settings to the user to select.

The language .tlf will include other files, called .tlp files.

The .tlf and .tlp files together form the translation for a particular language.

Use notepad++ or visual studio to edit .tlf files (they are in UTF-8-BOM format) as they are Unicode files.  Do not use an ASCII only editor.

Translation files can also be located for debugging purposes in the appdata/eddiscovery/translator folder.  A command line debug option can also be given to pick up translation files from anywhere.

# Format of translation files

Each line of the TLF/TLP is either a comment (//), blank line, Include statement or a definition.

A definition line translates one element, in the form:

ID : "English text example" => "Language text of translation of item"

IDs are sets of names using dots to separate.  They identify the text for a particular part of the program. These are always in English and you don't change them. ID is case sensitive and is generally in the form Module.Part.  The shortform .Part is also used which just means, assign it the previous stated module.

The English part after the colon is a guide for what you should be replacing.  Its not actually used in the program. It could be blank ("") for instance and EDD would ok: Warning: "" => "Warnung"

You will see in example-ex.tlf:

Systemnotknown: "System not known" @

The @ means an item has not received a translation yet. You should translate it. 

The program treats the @ different dependent on the Debug mode. In debug it repeat the program's internal English phrase but with quotes around it to show on screen the ID has been recognised.  In release mode it just repeats the programs internal English phrase exactly.

There are also in example-ex:

PopOutInfo.Journal.Description: "Journal grid view" => "\<Journal grid view\>"

The <> in the language text also means that the translation has not been done.

To translate, replace the @/text with => "Language text" with your translation.

For example, in the italiano-it.tlf file, you have:

Cancel: "Cancel" => "Cancella"

This translates the Cancel identity, which normally has the English text "Cancel" into Italian "Cancella".  And

PopOutInfo.Log.Description: "Program log" => "Registro del Programma"

This translated a PopOutInfo log entry into italian.

Translations are grouped together for particular panels/elements.  Not all of them needs translating, you may prefer to leave the more obscure bits in English.  A group will always start with the same prefix, for example AddOnManagerForm.<id>

# How to start

To start, copy the example-ex.* files found in the exe folder to a new set of names, such as francais-fr.*

Then start with the .tlf file and translate the generic UCs and the PopOutInfo.* entries.

Example-ex.* is the master source of translation Ids.  We keep them up to date with the source code. The other translation files are then based off of example-ex.  

Run EDD, your language should appear in settings | Languages.  Select it.  Close EDD and re-run.  Your translations should then be there - press the panel drop down button on the toolbar and the panel names should have changed to your text.

Then continue. EDDiscoveryForm and EDDiscoveryController are the next ones to do.  Then you can pick off the panels at your leisure.  The two .tlp files address the journal entries (affecting what's printed on the history panel) and the Materials/Commodity names.

Once you'd done a bit, please submit them back for inclusion!  Use discord to find out how.

# Format strings

You will see entries in c# or EDD Field builder format.  These show up due to {N} brackets or semicolons in the text.

c# format: Example is TravelHistoryFilter.Hours: "{0} hours" @

For C#, you need to keep the {N} entries in there (may be {0} {1} etc) but you may move them around to fix your translated text around them.

Field Builder format (1): Examples are:
JournalEntry.Capacity: "Capacity:;;0.0" @
JournalFuelScoop.Total: "Total:;t;0.0" @

The format is:
Prefix to item;Postfix to item;format control of item

You need to respect this.  Put your translated text in the prefix/postfix parts.  Leave the format control generally alone.

Field Builder format (2): Example are:
JournalEntry.NotLanded: "Not Landed;Landed" @
JournalEntry.Wanted: ";(Wanted)" @

The format is:

Text if false;text is true

Replace the text as appropriate.  The text may be blank, such as for the Wanted entry.

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

In debug mode, the translation system writes to appdata/eddiscovery/translator-ids.txt.  This indicates what files it reads and importantly tells you if any IDs are missing from the translation files.  If your based your files off of example-ex you should not have many of them.

# Advanced - use of EDDTest - Slightly Out of Date.  Mainly for Code editors.

Compile the EDDTest program, in the EDTools repo https://github.com/EDDiscovery/EDTools 

To find the .TX IDs in a set of source files, and to find the IDs used in the designer, use the following command line:

EDDTest scantranslate c:\code\eddiscovery *.cs c:\code\eddiscovery\eddiscovery\translations\ 2 italiano-it  >c:\code\output.txt

another:

c:\code\eddiscovery\eddiscovery>eddtest scantranslate . *.cs Translations\ 2 italiano-it showerrorsonly

without the translator:

c:\code\eddiscovery\eddiscovery>eddtest scantranslate . *.cs . . . showrepeats

these scan all .cs files under the subfolder set, and its sub folders.  Read in the italian translation files located at \..\translations\ (use the last slash) and use a 2 level up search for the TLP files, see above.  Output results to output.txt

Options available, list after the italiano-it bit, are: 

* combine - Use one list for local IDs across all files. Use in the journal folder. Don't use elsewhere.
* showrepeats - Show the repeats (they are normally removed)
* showerrrorsonly - use with the translator, only show lines where the translator file does not match the found ID.

You should scan all of the code under c:\code\eddiscovery.  It may be easier to do it a few sub folders at a time, instead of the whole thing.

Once run, it will scan the .cs files for designer type entries and for .Tx statements and produce a set of results such as below:
```
///////////////////////////////////////////////////// AddOnManagerForm in AddOnManagerForm.Designer.cs
AddOnManagerForm.buttonMore: "+" @ // OK
AddOnManagerForm.buttonExtGlobals: "Globals" @ // OK
AddOnManagerForm.buttonOK: "OK" @ // OK
///////////////////////////////////////////////////// AssignTravelLogSystemForm in AssignTravelLogSystemForm.Designer.cs
AssignTravelLogSystemForm.label1: "Travel Log System Name:" @ // OK
AssignTravelLogSystemForm.label2: "Date Visited:" @ // OK
AssignTravelLogSystemForm.label3: "New system name:" @ // OK
AssignTravelLogSystemForm.label4: "Travel Log Coordinates:" @ // OK
///////////////////////////////////////////////////// DraggableFormPos in DraggableFormPos.Designer.cs
DraggableFormPos: "DraggableFormPos" @ // NOT DEFINED

```

IDs found will be listed. If the translation is loaded, it will be checked against the translation file.  It will indicate if the ID is found (OK) or not found (NOT DEFINED) or if there is another error.

It will generally overstate the number of IDs to translate as it does not know about any programmatic exclusion of controls, such found in bookmarkform.cs which indicates not to translate certain controls using : 
            BaseUtils.Translator.Instance.Translate(this, new Control[] { labelX, labelY, labelZ, SurfaceBookmarks });

Use this as a good guide for what may be missing from your translator files, but don't rely on it 100%!
















