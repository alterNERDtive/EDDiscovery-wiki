# Defining Actions

Actions are small programs triggered by one of the action trigger conditions.  The programs allow you to reconfigure ED Discovery, to play a sound or voice synthesize a phrase. 

A trigger runs one program, which receives input variables to configure the program.

# Defining a new Action condition

.. pic

you define a new action condition:

* The first column defines ..

## Action triggers

* New Journal entries
* Program start (onStartup)
* Refresh start (onRefreshStart) and end (onRefreshEnd)
* New journal entry (one of the Journal event types)
* Keypress (onKeyPress)
* Voice recognition (to come)

## Associating a program

## Defining Input Parameters to the program

## Setting the condition for the program to run

Can be based on event parameters
Can be "Always true"
For keyevents, it should be KeyPress (== str or IsOneOf) key names. See below for key value names.

# Program variables

A program when run gets the following variables:

* User Globals 
 Dfined by the user in the Global dialog box

* Program information

 Commander - commander name

 RefreshCount - number of times refresh has been run on this commander. Reset to 1 when commander changes

 TriggerName - Event which caused the program to run.  The same as the event in the first column of the Action condition

 TriggerType - the main reason type why the program was run.  "ProgramEvent", "NewEntry", "KeyPress", "UserRightClick"

* Parameters in the event which causes the program to run 
 
 Any variables defined in the parameter field (just pass the P button) is passed to the event.  These parameters are associated with the action condition itself, not the program, so a single program can be assigned to multiple action conditions and have unique parameters passed in for each condition.  This is a powerful mechanism meaning you can limit the number of programs you need to write.

* Event information variables (if the program is run due to an journal event)

 Associated with the condition event which caused it to run.  Event data directly from the event JSON are named EventJS_<name>, event data decoded through the internal classes are named EventClass_<name>.  Often these will duplicate each other, sometimes the class names have better decoded information. The best way to see what is available is setting up an event, and running it (right click and run event) and using #pragma dumpvars * to see what is available.

 EventJS_event always gives the eventname, and EventJS_timestamp gives the time (US format).

*** Action Program Page

link to action doc

*** Running actions due to journal entries

