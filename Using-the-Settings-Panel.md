The settings panel configures operation of EDDiscovery.

![Settings page](https://imgur.com/BivPnFm.png)

The page is split into the following sections.

# Commanders
This grid shows you information on the list of commanders that EDDiscovery has stored information on.

It also allows you to edit the configuration of a commander and add or delete commanders.

See the topic [[How EDDiscovery Works|How EDDiscovery Works]] for information on how EDDiscovery discovers and creates new commanders. You can add a new commander manually, but that is not normally required any longer as EDDiscovery will make a new commander if it sees one in your journal logs.

The only use case for adding a commander manually is if you want to scan non standard folders for journal files. 

You can manually delete a commander. Note if the journal is scanned with the commander again, it will be auto recreated.

Clicking on Edit or Add will take you to the settings screen

![](https://imgur.com/7bFGwWc.png)

Here you can configure:

* Override Journal Location: Used in the remote EDDiscovery use case where you are running EDDiscovery from another computer and looking at the journal files on a file share. EDDiscovery will scan the folder given and read in all journal files found there.

* EDSM Integration: If you want to send your travel history to EDSM, you need to enter your EDSM Commander name, EDSM API key [[EDSM Integration|EDSM Integration with EDDiscovery]], and choose the sync directions you want to use.

* EDDN Integration: Select if you want to send information to the EDDN network (which you probably do if you like using EDDB etc since they rely on our data feeds)

* EGO Integration (TODO: requires updated image): If you want to automatically send discoveries to EGO, you need to enter your EGO login and API key [[EGO Integration|EGO integration with EDDiscovery]], and choose the sync directions you want to use.

* Frontier Companion API: If you wish, give your Frontier account log in details here (which is saved in encrypted form) and EDDiscovery will obtain information from the Frontier servers.  This is used primarly to obtain [[Market Data Panel|Using the Market Data Panel]] and drives that panels information. 

# Options

These configure EDDiscovery:

* Log HTTP requests: Store HTTP requests in a log in your APPDATA EDDiscovery folder.

* Number Rows Latest Entry Highest: By default 1 is the latest entry. If you prefer it the other way around, click this.

* Display Game time instead of local time: Display UTC game time instead of your local time.

* Show notification area icon : show a notification icon in the notification area.

* Minimize to notification area icon : when minimised, don't show a task bar icon, instead just show a notification area icon.

* Show UI Events in History. Certain UI events are reported to EDD by ED.  These occur frequently and are not really useful historically. Click on this to show them in history.

# Theme

See [[configuring ED theme|Configuring the look of EDDiscovery]] for how to change the look of EDDiscovery

# 3D Map Settings

You can configure some information that 3D Maps needs before starting here:

* Home System: What system do you want to call home?

* Open Centred on: Either home system or last History Grid selection

* Default Zoom: Select the zoom to use when opening. Use the map itself to find out your preferred zoom and then enter it here.

* Default Map Colour: New FSD journal entries are assigned this colour to show on 3D Map.

# Pop Out Widnow Options

* Load Setup on Start : Reload last saved pop out configuration

* Save Setup on Start : Save pop out configuration at exit

* Open Saved Setup : Open now the saved setup.  For manual use.

* Save Current Setup : Save now the current setup.  For manual use.

# Screenshots

The screenshot area allows you to configure EDDiscovery to automatically recognise screenshots taken either inside Elite Dangerous (F10) or via Steam, and convert and rename them into another format.  Additionally you can crop them if required.

The [[log|Using the EDDiscovery Log Panel]] during start up tells you what folder and file type it is scanning for, and after every screenshot tells you it has converted it.  Use this to check the system is working.

Screenshot previews are available in EDD by the [[screenshot panel|Using the Screenshot Panel]].

The master options are directly on the setting page:

* Auto convert: turn on/off screen shot system

* Remove original image after conversion: Select to delete the original screenshot (do not use for steam).

* Mark High Resolution Files: Add a marker to show in the filename its Hi Res (ED Screenshots only)

* Copy to clipboard: Copy the image directly to the clipboard, so you can paste it into other programs

Click on Configure to get to the detailed configuration dialog:

![Configure Screenshots](https://i.imgur.com/QTrEXwY.png)

Here you can set:

* ED/Steam Screenshot folder: Set this to the correct folder. See below.

* Store Converted Pictures: Where to put the files after conversion.

* Scan For: What files to scan for. Select BMP for ED launcher/ED, JPG/PNG (as selected by steam).

* Save As: What format to put the files in (note BMP cannot be used if the converted pictures folder is the same as ED screenshot folder)

* In Sub Folder: Option to store the file in a subfolder of store converted pictures, which different naming schemes.

* File Name Format: Use the drop down to select your preferred naming schema.

* Crop Image (and the settings): Cut the image to these specification.

## To select scanning for BMPs from Elite Dangerous F10 button

The correct folder for screenshots taken with Elite Dangerous is c:\users\<user name>\Pictures\Frontier Developments\Elite Dangerous.  Replace <user name> with your user name. Do a test screenshot and them ensure that .BMPs are in there from ED.

Save as JPG, PNG etc.  Do not select BMPs if the two folders are the same.

## To select scanning for Steam, you set up as follows:

Select Scan for JPG or PNG, dependent on your steam F12 settings. The correct folder depends on where you store your steam game files, but it should be Steam root folder/userdata/steam ID/ED ID/screenshots.

Save as JPG, PNG etc into a different folder than above. Do not delete the originals.









