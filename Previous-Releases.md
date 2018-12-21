# Previous Releases:

10.3.0 Was Released on December 11th 2018 for ED 3.3
See Release Notes for details.

10.2.0 Was Released on August 24th 2018 for ED 3.2.
See Release Notes for details.

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

## Very old notes for posterity:

Release log:

2016-04-13 Release 3.0.5

klightspeed: 3dMaps

Beeing able to show multiple maps on the Y=0 plane, and being able to filter by expedition or by date.
Add support for map textures to 3D map
Order maps by order clicked
Add ability to filter 3DMap visited systems by date
Camera now centers correctly on requested system again.
Improves the performance of the 3D map significantly by using Vertex Buffer Objects. This along with Vsync should give smooth movement using the keyboard.
Reduce the amount of CPU and GPU time being used when no movement is occurring, and stops the map being updated when the map window is not active, as requested in #60. This should also fix #161.

Set active commander when saving netlogs

Iainross;

Prevent error centring 3D map on nonexistent system
Merge remote-tracking branch 'blessed/master'
Prevent error clicking on header row of wanted systems list
Finwen:

Added a custom toolstrip renderer. To make theming of menues and toolsstrip (still some work to do)
Solved some exceptions usesers reported.
Added a button to show all stars on 2D Map.
Probably solved a expeption in 3D graph some users get then using a XBox controller.


2016-04-05 Release 3.0.4

Iainross:

3D Map is now centred properly and references lines drawn correctly when launched from the trilateration tab if default centre is set to Home System.
Added 3D Map button to Route tab, plotted route is drawn onto the map when launched from there.
Added 'Add to trilateration' context menu to Nearest Systems grid on Travel History control.
Added context menu to Distances grid on trilateration to copy systems to wanted systems list - local wanted systems are shown in the wanted systems grid, can be added to the distances grid by clicking and are persisted between sessions.
Added context menu to Wanted Systems grid on trilateration for deletion of locally added Wanted Systems.
Corrected check that systems are known on EDSM so it works again (site has started returning [] rather than -1 for bad system names)
Systems can be added to wanted from travel history

klightspeed: 3DMap updates
This adds the option for perspective rendering as an alternative to the current orthogonal rendering.
This also maps Right-drag to Y-axis translation, and Left+Right-drag to panning on the X and Z axes.
This adds the ability to see what star is at a given position in the 3D map, and to center the map on that star.
A single-click on a star will select the star, but not set it as the center system.
Double-clicking on a star will select the star, set it as the center system, and center the map on it.
It was suggested in #160 that when the centered system is changed, the camera angle should not change. This implements this, and also slews the camera in order to reduce confusion as to where the camera moved to.
This currently uses a sinusoidal velocity curve with a fixed 1 second slew duration regardless of distance or zoom. Clicking the mouse or pressing a movement button cancels the slew.

Finwen:
Fix rare exception in GetSystemsCount function
After 3d map was opened the close button failed to exit EDDiscovery


2016-03-23  Beta 3.0.0

* First version of Theme support. (Robby)
* Perform log file parsing using a regular expression Fixes  bug then ED logs  position incorrectly (Myshka)
* Prevent runtime error on deleting distance in trilateration. (Ian666)
* Check for actual current system when clicking the Trilaterate button (Ian666)
* Update to routing (Robby)
* Reduced memory usage for distances. (Finwen)

2016-03-13 Version 2.7.6
* Solve a DirectoryInfo exception then path is not valid.
* Get pushed systems from EDSM in a thread so UI do not need to wait for request..
* Show a messagebox if another EDDiscovery is running

2016-03-11  Version 2.7.5

* Changed EDSM sync option from Full/Push only to 2 checkboxes with ToEDSM/FromEDSM
* Shows Wanted systems from EDSM instead of Closestsystems for last known positions in tril tab.
* Support for DW4 map in 2DMaps
* Check so we only start one EDDiscovery (mwerle).
* Add Help -> About Box.
* Allot of improvments in Routing (Robby)
* Bug fix: with duplicate entries in Trilateration View (mwerle)
* Bug fix:  add additional checks for NULL system (mwerle)

* Lots of improvment in imageconversion from Robby
    Rewrite of the Image conversion to fix issues picking
    Problem with deleting files which have been cropped.
    Added more output file formats
    Fixed it so it renames them _1, _2 if multiples exist
    Can delete if you crop.
    Have checked it for cropping, deleting, both, all formats, BMP warning

* Trilateration UI improvements (mwerle)
* Allow sending distances to systems if current system has known coordinates without trilaterating (mwerle).
* Automatically copy "Last System" to clipboard when control is activated (mwerle)

2016-02-19 Version 2.7.4

* Removed systems from Proving ground
* Multicommander bug fix:  Forst commander did read EDSM api key from commander 2....


2016-02-17 Version 2.7.3

Robby: Can write note directly in the travelhistorylist now!
Mwerle : Trilateration: Tab skip over readonly fields So pressing tab in distance field moves you to next system name.
Iain: Option to only send travelhistory to EDSM.
Iain: Bugfix with logfiles passing over midnight.
Mwerle: Option to croop image on conversion.
Mwerle: Menu to copy selected systems from Travelhistory to trilateration.
Finwen: Better switching between multicommandes.
Finwen: Trilateration Tab to systemname copes name to clipboard (no need to do CTRL+C)


2016-01-03 Version 2.6.2

3DMap
* 3DMap now open maximized
* Created keyboard bindings (WASDG) to travel around in the galaxy.
* Can transform the camera in all directions and rotations
* Statusbar with information about position and more.
* Grid

2DMap
* Support for the new map of the whole galaxy made by Finwen and Marlon Blake


2016-12-28 Version 2.6.1

3dMap
*Show All known stars (on/off)
*Show all known stations (On/off)
EDDB:
*Bug: did not update system with population information from EDDB.
*Added in Admin menu a item to Force EDDB update.
EDSM
*Optional logging of EDSM communication


2015-11-04 Version 2.5.2
* Stores Travel log in local DB.
* Can sync Travellog with EDSM and sync log with several computers.
* Trilateration window enchanced. Copy systemname to clipboard on click. (No need to CTRL+C anymore.)
3D map in trilateration window shows lines to reference stars.
Added icons to Remove unused references and to remove all.


2015-09-04 Version 2.4.8
* Support for 2D maps made by Corbin Moran
* Autoconvert ED screenshots to png or jpeg and renames them to Systemname with time.
* Better integration with EDSM
* Trilateration is now better on suggesting good reference stars



2015-08-04 Version 2.3.7

* Moved trilateration to an own tab.
* Trilateration has a 3d star map button that show reference systems and suggested references-
* Star map works again
* Travel history age selection will remember the selection to next usage. And we added last 20 systems as option.
* EDStarCoordinator homepage has been down allot last days so we now have support for EDSM also.
* Moved status login to bottom of window.
* Can select installation directory


2015-07-10 Version 2.3.5

* The search box now moves when the window is resized
* New alternate installer instead of the auto updating click once installer. Also checks if new installer is available.
* 3d map did show government instead of normal plotting...


2015-07-10 Version 2.3.4

* Search in travel history. Search works on all fields. So you can search for a system name or something in your notes.
* Downloaded json files from EDDB and EDSC is now stored in appdata instead of current directory. This is for the the future (next version) alternative installer that will a more regular installer instead of the current auto updating clickonce installer. Both installers will be available.
* EDDiscovery should not xrach if netlogmain has invalid path

2015-06-26 Version 2.3.0

Together with Cmdr Majkl we have created allot of new things in this version.

* Trilateration routine to get coordinates for unknown stars.
* Eddiscovery also creates an AppConfigLocal.xml file to automatically to add verbose logging in ED.
* EDDiscovery starts faster with more work running in different threads.
* Easy way to add distance to next system.
* And a long list of other small bugfixes and small changes.






2016-06-18 Version 2.2.0

* Updates UI better during startuo.
* Travel history list is allot faster.
* EDDB integration. Get data about systems from http://EDDB.io Added 2 buttons to view a system in eddb or edit information i Ross.


2015-06-14 Version 2.1.27

* Allow regions with , as decimal separator to also use . as decimal separator
* Test button removed..
* Added more time span options (6 hrs, 12 hrs, 3 days, 2 weeks) - Thanks Majkl

2015-06-12 Version 2.1.26

* Much smaller installation package. Instead of bundling corrected TGC data from Redwizzard EDDiscovery now checks if a new version exists on my mirrored server and then download it on demand.



2015-06-10 Version 2.1.25
* Shows how many visits you have done to a system.
* Added some statistics Tolls menu and Statistics open up a form with some statistics. Will add more later.



2015-05-07 Version 2.1.22

* Refresh in travel history now gets new systems from EDSC.
* New corrected star database from Redwizzard.

2015-05-05 Version 2.1.21

* I had inverted Z axis in the 3d map. Should be correct now.
* Now shows coordinates for a system with full precision.



2014-04-24 Version 2.1.18

Only some small changes in this update

* Getting distances from EDSC in a thread -> EDDiscovery stars allot faster
* Added a menu. With links to forum threads and quick ways to open Elite Dangerous directory and the log file directory.

