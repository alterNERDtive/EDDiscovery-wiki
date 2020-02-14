EDD uses [[EDSM|https://www.edsm.net/]] to obtain details on star systems.  It checks after each EDD start and downloads new star data from EDSM when required.  This is all done automatically.

The [[settings panel|Using the Settings Panel]] has an option to disable this synchronisation if you wish to save bandwidth, and to limit what areas of the galaxy is stored to allow you to limit disk space used.

EDD also can send commander data to and from EDSM.  

A useful guide by Redfox is here at [Guide for Exploration Sharing](https://github.com/EDDiscovery/EDDiscovery/tree/master/Docs/Exploration-Guide-for-sharing-v2.pdf) which gives you a background on why you would want to use EDSM integration.

In order to send this data, you need to have configured an API key in EDD commander settings, obtained from EDSM.

Make sure that you have an account on [www.edsm.net](http://www.edsm.net). In EDSM go to the user drop down and select 'My API Key'  

![](http://i.imgur.com/6g8VGlZ.png)  

Now copy the numbers and and letters from the API Key  

![](http://i.imgur.com/VSwjmNh.png)  
 
Go to the settings panel, select the commander and hit Edit.  In the EDSM section, set your EDSM commander name (it may be different to your ED name, if not you can leave it blank) and the EDSM API you obtained.

EDD will sent your journal entries to EDSM to keep it up to date with your travels.  It will send all your jump history (slowly) to give it historical jump data.