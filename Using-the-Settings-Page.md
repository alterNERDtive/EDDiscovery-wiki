The settings page configures operation of EDDiscovery.

![Settings page](http://i.imgur.com/BeTNNbw.png)

The page is split into the following sections.

# Commanders
This grid allows you to configure information for commanders. 

See the topic [How EDDiscovery Works](How EDDiscovery Works) for information on how EDDiscovery discovers and creates new commanders.

You can add a new commander manually, but that is not normally required any longer.  The only use case for this is if you want to scan non standard folders for journal files. In which case, make a commander (any name will do) and set the override journal location to the folder where journal files will be written.  Then EDDiscovery will scan that folder and read in all journal files found there, creating commanders as required.  This is useful if your runnin EDDiscovery remotely from ED - share a network drive and EDDiscovery will work.

You can manually delete a commander. Note if the journal is scanned with the commander again, it will be auto recreated.

You may wish to configure a commander, for interaction with other systems as follows:

* EDSM API Key: If your going to send travel history to EDSM, you need to enter your EDSM API key [EDSM Integration](EDSM Integration with EDDiscovery).

* EDSM Name: If for some reason you did not use the same commander name used in game on EDSM, enter your EDSM name here.

* Override Journal Location: Used in the remote EDDiscovery use case above.

* Sync To EDSM: Click this on to send travel entries to EDSM.

* Sync From EDSM: Click this to get travel entries from EDSM into your history

* Sync to EDDN: Send selected events to EDDN.  The list of events is Trading data, outfitting, shipyear, stars.

# Options

These configure EDDiscovery:

* Log EDSM requests: Store EDSM requests in a log in your APPDATA EDDiscovery folder.

* Number Rows Latest Entry Highest: By default 1 is the latest entry. If you prefer it the other way around, click this.

* History cursor to new Journal Entry automatically: When a new journal entry is entered, change the cursor on the [history grid](Using the History Grid) to the entry.

* Display Game time instead of local time: Display UTC game time instead of your local time.

* Show notification area icon : show a notification icon in the notification area.

* Minimize to notification area icon : when minimised, don't show a task bar icon, instead just show a notification area icon.

# Theme

See [configuring ED theme](Configuring the look of EDDiscovery) for how to change the look of EDDiscovery

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





