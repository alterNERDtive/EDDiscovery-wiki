The edit add-ons menu provides the means to show what actions packs are installed, allow them to be enabled or disabled, and allow them to be edited.

Select Edit one of the packs from the menu and you can alter the conditions and events the packs respond to, and edit the programs.

![actions](http://i.imgur.com/gMhHyfu.png)

(Image out of date)

This shows two simple action events defined:

* The first, occurs on a keypress (column 1), and runs the program onKeyPress (Column 2).  The condition associated is when the KeyPress variable (which gets the name of the keypress when it happens) is equal to F6.  So we have associated F6 with the action program onKeyPress.

* The second, occurs when a journal event ApproachSettlement is received by EDD.  It runs the program ApproachSettlement. We could set up a condition to check for a parameter of Approach settlements is true, and only allow the program to run if so (say EventClass_Name == (Str) settlement name) but here we have used the condition Always True, which means when any ApproachSettlement journal event is received, the program runs.

You can add as many event conditions as you like (see the voice pack for instance). You don't have to have a unique program per condition, you can share programs and let the program adapt to the event (see GenericResponse in voice packs).  You can add multiple conditions.

The other options on this screen are:

* Plus (at end of list) : add another event
* Sort/Sort2 : Sort the events. First option is by event name, then program name.  Second is by Condition value, then event name.
* X : delete event
* Plus (on right) : Add another condition
* Up Caret : move event up one

Along the bottom are some controls for the event packs as a whole:

* Set: name drop down box : This is how you make a new pack (using New) or go to another pack for editing. Changing from one pack to another causes the current pack to save (you may get a warning if it detects errors) and then the other packloads.
* Enable : Enable or diable this pack, as per the [[Manage Add-ons|Using the manage Add-Ons Menu]] menu.
* Program : directly edit a program, or make a new program (You may want a program not directly associated with an event if its a subroutine)
* Globals : Edit the EDD global action variables.  These feed information into actions.  For instance the speech parameters are global variables which you can edit here (but thats easier using [[Speech Synthesis Settings|Using the Speech Synthesis Settings Menu]]

Clicking on 'P' for program beings up the editing box to allow you to define the program:

![Program edit](http://i.imgur.com/tYAZ20P.png)

Here you can edit a program.  This program has two statements, a Print and a Say command.  You can add more statements using the + button, configure each statement using the 'C' button, and use ^ to move the statements around.

You can rename the program if required.  If so, the current program is left alone and a new program is made.

You can delete the program using the 'X' under the close icon at top.

Left click drag and right click allows statements to be highlighted then copy/paste/deleted.  Make sure your dragging across empty screen areas, it won't work if your on top of a control like the text box.  The area between the statement name and the statement value is best.

![copy paste](http://i.imgur.com/uLlzabM.png)

Left click drag to highlight, then click copy.  Right click on the place to insert above (make sure its empty screen space), then paste.

You can also ask for whitespace to be inserted between statements for clarity.

Along the bottom are some controls for the program:

* Text Edit : Edit in a text editor.  This is a more advanced option. EDDiscovery will write the script to a temporary location.  It will launch your text editor.  Your edit it.  Then you must save the file back to disk and quit your text editor.  Once EDDiscovery sees the text editor has been closed, it then re-reads the file and checks it. Any problems will be notified and you can then correct them in the editor if you choose.  Remember, make sure you save the file back to disk before quitting otherwise EDD won't see the changes!

![text edit](http://i.imgur.com/VIveDYQ.png)

* Load : Load a text version of the program
* Save : Save a text version of the program

The power of this system comes from using the variables defined by events, such as EventClass_Name etc. 

This [action program language google document](https://docs.google.com/document/d/1M7ODl9Z68vzKCRFXKD2be3l3747G_rgzM1TnaXOiR0w/edit?usp=sharing) describes the action program language.