From 10.2, EDD supports multiple languages for its user interface.  You can change the language in Settings.

Language translations are provided by the EDD user community.

Not all sections of the program may have all items translated.  There are a very large number of items to translate so it may be that the author of the translation only concentrated on the primary parts.

## Your language not there? Translation not complete?

Then contribute!

Language translation files are simple.  They are found inside (for the release version) the .exe folder (c:\program files\eddiscovery\eddiscovery normally). 

The primary translation for a language is called a .tlf file, and is named <languagename>-<iso 2 or 3 char code>.tlf.  For instance italiano-it.tlf.  Any language files found in the .exe folder using the .tlf and this format name will be presented in settings to the user to select.

The language .tlf will include other files, called .tlp files.

The .tlf and .tlp files together form the translation for a particular language.

Use notepad++ or visual studio to edit .tlf files (they are in UTF-8-BOM format) as they are Unicode files.  Do not use an ASCII only editor.

# Format of translation files

Each line of the file translates one element, in the form:

ID : "English text example" => "Language text of translation of item"

IDs are sets of names using dots to separate.  They identify the text for a particular part of the program. These are always in English and you don't change them. 

You will see in example-ex.tlf:

Systemnotknown: "System not known" @

or

PopOutInfo.Journal.Description: "Journal grid view" => "<Journal grid view>"

The @ or the text in <> in the language text means that an item has not received a translation yet.  To translate, replace the @/text with => "Language text" with your translation.

For example, in the italiano-it.tlf file, you have:

Cancel: "Cancel" => "Cancella"

This translates the Cancel identity, which normally has the English text "Cancel" into Italian "Cancella".  And

PopOutInfo.Log.Description: "Program log" => "Registro del Programma"

This translated a PopOutInfo log entry into italian.

Translations are grouped together for particular panels/elements.  Not all of them needs translating, you may prefer to leave the more obscure bits in English.  A group will always start with the same prefix, for example AddOnManagerForm.<id>

# How to start

To start, copy the example-ex.* files found in the exe folder to a new set of names, such as francais-fr.*

Then start with the .tlf file and translate the generic UCs and the PopOutInfo.* entries.

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









