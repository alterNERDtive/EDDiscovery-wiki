# Previous Releases:

10.1.0 Was Released on 14th June 2018 for ED 3.0.X

* INARA
* DLL Integration
* History Limit Loading
* Lots of other goodies - see the release notes.

Voice pack V8 is for this version - please update!

10.0.X Was Released on 9 May 2018 for ED 3.0.X

* New panels, new Splitter support for configurable splitter windows

* Lots of other goodies - see the release notes.

9.1.8 Was Released on 20 Mar 2018 for ED 3.0.3

9.1.0 to 9.1.4 have a bug which prevent the auto upgrade message from showing!  Please move to 9.1.8.

See [[Release Notes|https://github.com/EDDiscovery/EDDiscovery/releases/latest]]

* ED 3.0 support for new journal entries

* Compass panel/Bookmark panel for new planetary bookmark features

* EDSM Star database fully controllable over storage and download

* Lots of other goodies - see the release notes.

9.0.3 Was released on 17 Jan 2018 for ED 2.4 

See [[Release Notes|https://github.com/EDDiscovery/EDDiscovery/releases/tag/Release_9.0.3]]

* [[Free Voice Control|Free Voice Control]] - control Elite using your microphone!  Install the FVC action pack, make sure you have key bindings set in elite for items you wish to voice control, and talk away!   Over 140+ voice commands built in!  You do not need Voice Attack to use this functionality, its stand alone.

* Map/Plot panels added

* Fix up of various issues

9.0.1 was released on 19 Dec 2017 for ED 2.4

* [[Free Voice Control|Free Voice Control]] - control Elite using your microphone!  Install the FVC action pack, make sure you have key bindings set in elite for items you wish to voice control, and talk away!   Over 140+ voice commands built in!  You do not need Voice Attack to use this functionality, its stand alone.

* [[Scan Grid|Using the Scan Grid]] added

* Synthesis/Engineering/Shopping list tabs are improved with more options

* Numerous minor fixes to bugs.

* Voice Pack updated with more fixes.

9.0.2 was released on 9 Jan 2018 for ED 2.4 

* [[Free Voice Control|Free Voice Control]] - control Elite using your microphone!  Install the FVC action pack, make sure you have key bindings set in elite for items you wish to voice control, and talk away!   Over 140+ voice commands built in!  You do not need Voice Attack to use this functionality, its stand alone.

* [[Scan Grid|Using the Scan Grid]] added

* Synthesis/Engineering/Shopping list tabs are improved with more options

* Voice Pack updated with more fixes.

9.0.2 fixes numerous small issues, see the release notes.


8.4.X was released on 2 Nov 2017 for ED 2.4.

* Configurable tabs to the program. Right click on the major tab and add/remove tabs. The program starts with a more limited set of tabs - use right click on the tabs to add your chosen ones back.
* Exploration panel updates
* Many under the hood changes to improve panel output, to improve responsiveness etc.

8.3.X was released on 26 Sept 2017 for ED 2.4.

* Companion API (CAPI ) was temporary disabled in early ones of this sequence.  Now re-enabled in the latest 8.3.X. Due to Frontier CAPI API changed after ED 2.4 release.
* Added support for new journal event from Elite Dangerous 2.4
* New Shoppinglist control with transparent overlay
* Added popout control to list estimated scan values for bodies in system
* Send Materials, Data and Cargo to EDSM
* Move screenshot settings tab to settings panel, removed import/export tab and incorporated features on appropriate panels.
* Remember to Download Voicepack V5 and JMKV2 for latest support of ED 2.4
* Moved functionality to excel icons on route/history/scan and admin menu. Export page removed. Moved to move logical UI positions.
* CAPI can be disabled without losing the credentials.
* Added visit count to UC star distance, some UC clean ups with events
* Added a new "TransparentClickThru" transparency mode for popup windows.
  * Designed for mouse pilots that want panels overlapping their Elite: Dangerous window, but are tired of focus stealing.
  * Requires holding down a certain key (default: <kbd>shift</kbd>, but editable in settings) in order to focus the window.

8.2.X Released was released on 11 August 2017 for ED 2.3

* New! 8.2.3 Adds a [[safe mode option|Safe Mode]].  Hold down shift key and run EDD and a safe mode dialog will appear, which allows you to run without remembering window positions, without loading a theme, or to move your databases to another folder or drive.
* UI major rework, tooltips, drop down menus etc optimised.
* The Grid major tab added, allows any of the panels to be placed at any position on it
* Grid Pop outs supported, allows you multiple pop outs of any set of arbitrary panels
* Toolbar at the top added, which can roll up to minimise screen space.
* System info panel added, fully configurable, will work in transparent mode. Much more information.
* History page now consists of a fixed travel grid, and four configurable panes (one bottom, three left).
* Travel grid and journal grid have their own 'Cursor to top' options instead of one global option.
* Uploads to EDSM credits, current ship, progress, rank
* Elite galaxy online integration (EGO)

8.1.X was released on 10 july 2017. [Download here](https://github.com/EDDiscovery/EDDiscovery/releases). This features:

* Supports the [[Joystick Keyboard Mouse|Using the JKM Pack]] pack adding vocalisations to your input devices
* Supports the [[OBS Pack|Using the OBS Pack]] to provide OBS overlays
* Supports the [[SoundBlaster|Using the SoundBlaster Pack]] pack to play sounds when journal events occur
* Updates the [[voice|Using voice packs]] pack to add many more events and adds NPC voices into the pack
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

8.0.X Was released on 9 may 2017. [Download here](https://github.com/EDDiscovery/EDDiscovery/releases). This features:

* Added Companion API (CAPI) login (login in to Elite Dangerous Web API) this will provide:
* Market Data Panel showing commodity prices
* Storage of commodity prices in the journal so you can see the price at a given station
* Autosend commodity prices to EDDN at docked Event.

Also:
* Commander dialog added for commander settings with CAPI login details
* Many engineering recipe fixes.
* On scan panel lava icon temperature limit increased.
* Distance tooltips are to systems, not planets.
* Show home system directly in the tooltip.
* Add SuperMassiveBlackHole star type (for Sgr A*)
* Name M and MS stars
* Removed some EDDN start/end sync spam in log
* Catch errors reading register from EDDUser.sqlite Don't error out when EDDUser.sqlite exists but has no data.
* Context menu: copy journal entry to clipboard
* Merge fuel scoop events
* Prevent error selecting None for levels or material filters
* Added more journal events 

7.0.X was released to coincide with 2.3 Commanders (11 April 2017). This featured:

* [[New Load out panel|Using the Load Out Panel]] with Coriolis integration.  Track the modules on your ship. Export to Corolis (excepting any Engineer modifications which Frontier does not currently tell us above via Journals)
* [[New Synthesis panel|Using the Synthesis Panel]].  Show what enhancements you can make with your available resources. Set up a wish list and it will tell you want you can make and what you need to make more.
* [[Updated voice support|Using voice packs]] for all new journal events
* [[New Mission panel|Using the Missions panel]].  Display current missions and past missions, total rewards.
* Ship information is sent to EDSM
* Improvements to importing systems into trilateration
* New 2.3 Journal entries added.  
* Lots of effort into normalising and making the journal data human readable.
* Voice pack updates to voice pack 3

7.0.2 adds on:
* [[New Engineering panel|Using the Engineering Panel]].  Show what blueprints you can make with your available resources. Set up a wish list and it will tell you want you can make and what you need to make more.




# 6.1 for ED 2.2
* more [[voice packs|Using voice packs]] features, which add speech to EDD. This has voice effects to make your computers voice more fun to use, verbosity control, EDSM read out of known system data, better read out of star names etc.

* Audio device can be selected

* Minor changes to [[key packs|Using key packs]] to add a few more key shortcuts.

* Stability fixes and speed improvements

* Scan data estimated value added

# 6.0 for ED 2.2

* [[voice packs|Using voice packs]] to add speech to EDD

* [[key packs|Using key packs]] to add key shortcuts, 

* [[Actions|Using Actions]] to define your own custom responses to key presses or journal entries, 

* Many visual improvements.

* refinements to journal output.

## 5.0 and previous

See the github release history
