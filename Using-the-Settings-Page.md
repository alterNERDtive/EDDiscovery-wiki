The settings page configures operation of EDDiscovery.

![Settings page](http://i.imgur.com/PGcYUQi.png)

The page is split into the following sections.

# Commanders
This grid shows you information on the list of commanders that EDDiscovery has stored information on.

It also allows you to edit the configuration of a commander and add or delete commanders.

See the topic [[How EDDiscovery Works|How EDDiscovery Works]] for information on how EDDiscovery discovers and creates new commanders. You can add a new commander manually, but that is not normally required any longer as EDDiscovery will make a new commander if it sees one in your journal logs.

The only use case for adding a commander manually is if you want to scan non standard folders for journal files. 

You can manually delete a commander. Note if the journal is scanned with the commander again, it will be auto recreated.

Clicking on Edit or Add will take you to the settings screen

![](http://i.imgur.com/iHMQX8k.png)

Here you can configure:

* Override Journal Location: Used in the remote EDDiscovery use case where you are running EDDiscovery from another computer and looking at the journal files on a file share. EDDiscovery will scan the folder given and read in all journal files found there.

* EDSM Integration: If your going to send travel history to EDSM, you need to enter your EDSM Commander name, EDSM API key [[EDSM Integration|EDSM Integration with EDDiscovery]], and choose the sync directions you want to use.

* EDDN Integration: Select if you want to send information to the EDDN network (which you probably do if you like using EDDB etc since they rely on our data feeds)

* Frontier Companion API: If you wish, give your Frontier account log in details here (which is saved in encrypted form) and EDDiscovery will obtain information from the Frontier servers.  This is used primarly to obtain [Market Data Panel](Using the Market Data Panel) and drives that panels information. 

# Options

These configure EDDiscovery:

* Log EDSM requests: Store EDSM requests in a log in your APPDATA EDDiscovery folder.

* Number Rows Latest Entry Highest: By default 1 is the latest entry. If you prefer it the other way around, click this.

* History cursor to new Journal Entry automatically: When a new journal entry is entered, change the cursor on the [[history grid|Using the History Grid]] to the entry.

* Display Game time instead of local time: Display UTC game time instead of your local time.

* Show notification area icon : show a notification icon in the notification area.

* Minimize to notification area icon : when minimised, don't show a task bar icon, instead just show a notification area icon.

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





