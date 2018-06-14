From EDD 10.1, EDD supports loading a 3rd party DLL (Dynamic Link Library, a form of portable application extensions)

3rd party DLL will normally be distributed along with a action pack, installed using the [[Add-On menu|Using the manage Add Ons Menu]].  

Users must be aware of where the DLL comes from and use their own judgement if to use it.

This [[repository on git|https://github.com/EDDiscovery/EDDiscoveryAdditionalDLLs]] has an example DLL and a harness to demonstrate how to write a 3rd party DLL.

You can remove the DLL either by deleting the action pack that it came with, or using [[Safe Mode|Safe Mode]] to delete all DLLs.

3rd Party DLL interface is defined in [[this file|https://github.com/EDDiscovery/EDDiscoveryAdditionalDLLs/blob/master/ExampleAddInDLL/Win64DLL/EDDInterface64.h]].  Please refer to that for detailed on the functions EDD uses and the callbacks you can make to EDD.

Any 3rd party DLLs distributed within the EDD distribution system for add on features will need to conform to the following rules:

* Open source code, nominally using the Apache License (others may be considered).  You can host on your own GitHub/GitLab etc host, or you can send the source code and we will host on the EDDiscoveryAdditionalDLLs github project.  Source code will be reviewed before it is acceptable.

* Use of well known 3rd party DLLs only (from reputable vendors/NUGET packages etc)

If you wish to distribute outside of the EDD distribution system then EDD project can't control that.  
