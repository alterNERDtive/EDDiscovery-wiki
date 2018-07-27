10.2 adds in support for multiple languages


* How It works

To define a language, a languagename-isotwocharname.tlf file needs to be present either in the .exe folder where EDD is run from (the installer puts these files in there) or in the appdata/eddiscovery/translator folder.

The TLF file defines language strings for all EDD panels, forms, program features etc.

The TLF must be in UCS-BOM-8 format.  Use only notepad++ or visual studio to edit it.

The TLF file may use Include filename to include another file (usually called TLP files)

* Structure in the EDD Solution (Visual Studio)

In EDDISCOVERY project, the VS folder Translations contains the source controlled TLF files.  

In EliteDangerous project, the EliteDangerous subfolder contains TLP file containing definitions for the Materials and other common ED terms

In EliteDangerous project, the EliteDangerous subfolder contains TLP file containing definitions for the Materials and other common ED terms




