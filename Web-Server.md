EDD 11.0 supports a web server.  This can serve pages to your tablet or laptop.

Enable this feature in [[Settings|Using the Settings Panel]].

This feature has been tested in Windows/Chrome, Windows/Firefox, Android Chrome.  

There may be rendering issues on other browsers or on other hardware.  Browsers implementation of HTML/CSS is not uniform.  Use the latest version of the browser on your platform.

# Turning On Web Server

By default web server is off.  To enable, click the enable check box.

EDD will ask you if you wish to open the windows firewall to allow this feature to work.  To enable EDD to serve webpages, we need to ask windows for permission to serve on the port selected, and to open a firewall rule to allow the port to pass through the firewall.  

You only need to do this once per port number.  If your running as a normal user windows will ask you for the password of the admin/superuser to allow the operation to complete.

If EDD webserver is not working, or working only on the PC but not from a tablet, its because the firewall rule has not been set up.  EDD can configure the windows firewall.  If you are running another type of firewall you'll have to do this manually.  Set up a inbound rule to allow TCP traffic on the port number to go to EDD.

Use the test button to see if the configuration is successful. This will open a browser window which EDD should serve web pages to.

# Journal Page
This shows the journal view and the current status (like the system info panel).

![](https://i.imgur.com/BCQHkCu.png)

The journal view can be scrolled up and down.  Clicking on the event image changes the status to that entry.

#  Status Page

This shows the current status and a set of icons describing the state. At the bottom are action buttons where you can send orders to EDD to perform actions, such as landing gear down, lights on, etc.

The icons change dependent on the game mode.

## In Supercruise:
![](https://i.imgur.com/QBfV3Ww.png)

Indicators: Docked, Landed, Shields, In Wing, Fuel Scooping, Low Fuel, Heat Damage, In Danger, Being Interdicted, Charging FSD, FSD Cooldown

Actions: Lights, Hardpoints, Supercruise, Supercruise/Jump, Orbit Lines, Previous Target, Next Target, Target Next System in Route, Previous fire group, Next Fire Group, Increase Systems Power, Increase Engine Power, Increase Weapon Power, Balance power, Galaxy map, System map, Take picture.

## In SRV:
![](https://i.imgur.com/mirb5Ho.png)

Indicators: Under ship, low fuel, Shields

Actions: Handbrake, Turret, Drive Assist, Lights, Recall Ship, Increase Systems Power, Increase Engine Power, Increase Weapon Power, Balance power, Galaxy map, System map, Take picture.

## In Normal Space:
![](https://i.imgur.com/OYc34DR.png)

Indicators: Docked, Landed, Shields, In Wing, Low Fuel, Heat Damage, In Danger, Charging FSD, Mass locked, FSD Cooldown

Actions: Landing Gear, Lights, Flight Assist, Hardpoints, Cargo Scoop, Night Vision, Boost, Shield Cell, Chaff, Heatsink, ChargeECM, Supercruise, Supercruise/Jump, Orbit Lines

Line 2: Previous Target, Next Target, Highest Threat, Previous Highest Threat, Next Highest Threat, Previous subsystem, Next subsystem, Previous Fire Group, Next Fire Group, Increase Systems Power, Increase Engine Power, Increase Weapon Power, Balance power, Defensive Behaviour

Line 3: Agressive Behaviour, Focus on Target, Hold Fire, Hold Position, Follow me, Request Dock, Open orders, Galaxy map, System map, Take picture.


# Grid Page
This shows the status icons and action buttons from the status page, but larger, and easier to hit on a tablet. This page acts as a super Roccat style grid with interactivity with the game.

![](https://i.imgur.com/sLyQlIw.png)

# Additional In Wing Buttons

You can target wingman 1 to 3, target the wingman's target, and target his next system.  These appear only when in wing.

![](https://i.imgur.com/sca5CD9.png)
