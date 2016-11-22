Welcome to the EDDiscovery wiki!

# EDDiscovery – What is it? 

You play Elite Dangerous and have heard of EDDiscovery - and ended up here.  So what _is_ it?  
  
In short it’s a 3rd party tool that can track your Elite Dangerous travels, combat, trading, rank etc. Before Elite Dangerous 2.2 it could only track travel, now with 2.2, EDDiscovery tracks much more! It can now log other data such as rank, commodities, materials, scans and all host of other data.

EDDiscovery also gives you a 3D and 2D maps of the galaxy, showing travel history and data from EDSM and EDDB to aid your journey through the Elite Dangerous galaxy.

Here’s an example of the history page using the ED Theme Elite Verdana:
![](http://imgur.com/a/T09Gh)  



  
But whilst a list of visited systems is useful, lets be honest, it's a bit boring.  EDDiscovery takes these visited systems and plots them on series of high quality 2D maps.  Here's an example:  
![](http://i.imgur.com/8XihLab.png)  
  
Yes, those coloured lines are my travels, and yes you get to pick the colours :)  You may have noticed the coloured squares earlier in the travel log - they correlate to the lines on this map.  
  
But wait...there's more!  
There’s also a 3D version of your travels – note the plot colours are the same:  [The blue blob is basically ‘the bubble’ – each system that has a station is coloured blue by default]  
![](http://i.imgur.com/X9o9Jbp.png)  
  
In case it is not obvious from the above – not all systems are shown.  In fact of the ~100 billion (that’s 100,000,000,000), only a little over 150,000 are currently shown.  Why?  Maybe you should read on a little into the ‘how it works’  
  
# How it works
The travel log bit works off your gaming log files.  You may have heard the term ‘verbose logging’ before.  By default, ED creates a very basic log file each time it runs.  Enabling verbose logging means the logs are filled with a lot more information – including the name of the system you are currently in.  
  
So EDD constantly checks the log file for updates and retrieves the system name.  That’s it is able to create the travel log.  If you previously enabled verbose logging, EDD will even run through those logs and populate the travel log from your history.  Do note that there is no way to get this info if verbose logging is not enabled.   If you start the tool before the ED launcher, the tool will enable verbose logging for you :)
  
When you run EDDiscovery, you may notice a mix of blue systems and black systems.  
![](http://i.imgur.com/lRlK2EA.png)  
The black systems are the ones that have known positions (X, Y, Z co-ordinates) whilst the blue ones do not.  You turn a system from blue to black through a process of ‘trilateration’ – we’ll look more into that in the usage guide.  
  
If you recall the earlier maps, the points are plotted against the black systems.  After all, if we don’t know where a system is, we can’t plot it right?   Now, remember number 150,000?  That’s the number of black systems – ie, the ones that have known X, Y, Z co-ordinates.  If you look at the screenshot, you’ll see the co-ordinates for the highlighted system are (ignoring the decimal for easier reading) 4417, 857, 37898.  As an added bonus, EDD also tells us the system is 38,164 ly from Sol.