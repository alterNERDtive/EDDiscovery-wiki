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


# Key Actions
To define a key action, the trigger event needs to be onKeyPress, the condition must be in the form KeyPress string equals (or IsOneOf) and either a single keyname (string equals) or a comma separated list of keynames (IsOneOf)

Keynames are:

* Shift+ , Ctrl+ , Alt+ , Shift+Ctrl+, Shift+Alt+, Shift+Ctrl+Alt+

* A-Z, 0-9

* Numpad 0-9

* Oem1 (';' on UK keyboards)

* Oem5 ('\' on UK keyboards)

* Oem7 ('#' on UK keyboards)

* Oem8 ('`' on UK keyboards)

* tidle, comma, period, question, Minus, Plus, Home, End, Insert, Delete, Next (Pagedown) PageUp, Back, Down, Up, Left, Right, F1-F12, Decimal, Return, Enter, Add, Subtract, Multiply, Divide

# Action Program

link to action doc



