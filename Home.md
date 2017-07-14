# Current Version

8.1.X released on 10 july 2017 is the current version - try it if you wish. [Download here](https://github.com/EDDiscovery/EDDiscovery/releases). This features:

* Action Menu Improvements
* CSCore back to nuget package, added mouse input
* Added Missions event info, changed info to basic ship info on events.
* Fixed bug in writing event line with comma in condition
* Fixed major bug in missionlists - new entries was losing the data
* Historylist has been cleaned up and re-orged into sections. Only real change is addition of Copy() to handle copying the class from one to another properly, for use in eddiscoverycontroller
* Prevent some overflows in WndProc
* CAPI checks for forbidden and login url
* Improved expired session fix
* EDDN ignore item >1day old.
* Remove incorrect cmdr set in HL and protect them

* Fix EliteBindings, Add in Perform listeliteinput, allow input device to be listed
* Added in %isPresent to help with the voice menus,
* Sped up scan of logs to every 500ms, added in to config dialog drop down combo
* AboutForm Updates
* Add galmap name fields to Route tab
* Translate Earthlike world to journal format name.
* More code to support NPC voices
* Allow audio mixing in SAY during speech
* Small fix to prevent failure if prev packs not present during install
* Add last dock to travelhistory/journal.
* Add EDSM buttons to target control on travelpage and to route finder
* #1106 fix radians in axial tilt
* #990 allows body name in screenshots
* In Stats panel also show stats since last dock.
* Stats panel: Add custom from and to date for Scans and Travel tab.
* Fix bug in audio subsystem when doing priority inserts

Also see [[Previous Releases|Previous Releases]] for past history of EDDiscovery.

# Troubleshooting
See [[Troubleshooting|Troubleshooting]]

# EDDiscovery - What is it?

You play Elite Dangerous and have heard of EDDiscovery - and ended up here.  So what _is_ it?  
  
In short it's a 3rd party tool that can track your Elite Dangerous travels, combat, trading, rank etc. Before Elite Dangerous 2.2 it could only track travel, now with 2.2, EDDiscovery tracks much more! It can now log other data such as rank, commodities, materials, scans and all host of other data.

EDDiscovery also gives you a [[3D map|Using the 3D Map]] and [[2D maps|Using the 2D Map]] of the galaxy, showing travel history and data from EDSM and EDDB to aid your journey through the Elite Dangerous galaxy.

Here's an example of the history page using the [[ED Theme Elite Verdana|Configuring the look of EDDiscovery]], EDDiscovery supports themeing the user interface to your specification.

![](http://i.imgur.com/gAxIRN8.png)

The main user interface of ED consists of a set of tab pages

* [[History|Using the History Page]] : The history page supports four selectable [[Panels|Using Panels]] which you can select what information is displayed.
* [[Journal|Using the Journal Page]]
* [[Trilateration|Using the Trilateration Page]]
* [[Screenshots|Using the Screenshots Page]]
* [[Route|Using the Route Page]]
* [[Route/Expeditions|Using the Route Expeditions Page]]
* [[Export|Using the Export Page]]
* [[Settings|Using the Settings Page]]

Which you can select from. See the topics above for information on each page.

EDDiscovery also has [[Menu Options|Menu Options]] for some quick access functions and to run housekeeping functions which seldom need executing.

[[Configuration Options|Configuration Options]] exist to control how EDDiscovery starts and where data is stored.

You can learn how [[EDDiscovery works with Elite Dangerous|How EDDiscovery Works]] here.

See the sidebar to the right for other topics.

# Images:
Some images are screenshots from Elite: Dangerous © 2012-2016 Frontier Developments plc. All rights reserved.