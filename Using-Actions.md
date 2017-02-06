# What are Actions and Action Programs and Packs?

The Action system, new to 6.0, adds the ability to run a small program when an event is received via the journal, or via a keypress, or due to a program event (startup,shutdown, popup etc).

The action language itself is described in this [action program language google document](https://docs.google.com/document/d/1M7ODl9Z68vzKCRFXKD2be3l3747G_rgzM1TnaXOiR0w/edit?usp=sharing) as it is too complicated to describe on this simple wiki.

These programs can trigger program events themselves, say phrases to the windows text to speech engine, play a sound etc.

Using Actions makes it possible to make action packs. An action pack is a combination of the event triggers and the programs which support those triggers.  Various action packs are in existance, the most common ones is the voice pack (adding voice output to EDD) and the keyboard pack (adding ctrl and F key presses to EDD).

Access to the actions system is via the Add-Ons menu (because these are optional add-ons to the system).  The menu defines:

* [Manage Add-ons](Using the manage Add-Ons Menu) : Allows the user to install, remove or enable/disable the add on packs.

* [Edit Add-on Action Files](Using the edit Add-On Action Files Menu) : Allows creation of add-on packs.  Also see [Actions](Using Actions)

* [Speech Synthesis Settings](Using the Speech Synthesis Settings Menu) : For the speech pack, a user friendly menu to configure various speech parameters.

* [Edit in text current speech synthesis variables](Using the edit Speech Synthesis Variables Menu) : For the speech pack, a quick way to go to the definition file for the speech variables

* Stop currently running Action program : Only use if a program with a loop continues and refuses to stop (unlikely).

Click on one of the above to see how to download and configure an action pack.


