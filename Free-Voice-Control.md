This pack allows you to use voice commands to control Elite.  You can order landing gear up, hyperspace,
lights on etc.

NOTE: You do not need Voice Attack to use this functionality, it's stand alone.

You can find all the commands supported by using Help | Free Voice Control Help menu option.

You need to make sure any commands you want to say has an equivalent key binding in Elite Dangerous. A joystick binding won't work, it needs to be a keyboard key (due to Windows limitations). EDD will warn you if it can't find a key binding for a particular phrase - check the log window.

EDD reads the keybindings file at startup.  If you change them in Elite, for now just restart EDD to pick the new ones up.

**Note that you need to make Elite create a key bindings file **- if you use one of the stock bindings then it won't have written the file.  Just go in to Elite and manually create a key binding on a function (does not matter which one) and it will create a custom key binding file which EDD will see.

Windows voice recognitions is very sensitive to the following:

* That you trained your voice (use Control Panel | Sound (Win7) or Speech Recognition (Win10)) to train it
* That you have the right volume level for your microphone (Control Panel | Sound, click on the mic and set the levels)
* That there is minimum other noise the microphone can hear

Getting it set up right can sometimes be a bit of a challenge.

Currently the voice pack supports only the default recording device, set this in Control Panel | Sound | Recording\r

You may want to enable in the Free Voice Control Configuration the \"Show failed voice recognition\" and see what its listening to in the log window.

Enjoy.

PS. I have plans for a standalone FVC program - watch out for that.