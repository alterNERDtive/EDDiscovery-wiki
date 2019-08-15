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

# Web Pages