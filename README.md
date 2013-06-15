hadoop-eclipse-plugin-1.2.0
===========================

eclipse plugin for hadoop-1.2.0

Software Requirements:
jdk >= 1.6.0_45  //So just use jdk1.7
ecilpse >= juno

The environment is accessible through the "Map/Reduce perspective" (the blue elephant icon in the top-right side of the main window). To open this perspective, select the menu: Window, Open Perspective, Other, and finally Map/Reduce. This perspective is roughly a Java edition environment extended with:

    a view named "Map/Reduce locations" which lists Hadoop locations (the view at the bottom of the main window),
    a file browser for the distributed file systems associated to each Hadoop locations (on the left side). 

Hadoop Map/Reduce locations

The location view allows the creation, edition and deletion of Map/Reduce locations.

To create a new location click on the "New Hadoop location..." button in the view toolbar or in the contextual menu.

A wizard pops up and asks for the location parameters.

You must at least fill the following entries:

    the location name (avoid ponctuation marks),

    the masters addresses: hostname or IP address and TCP port numbers for the Map/Reduce master (the JobTracker) and for the Distributed File System (the NameNode). 

The Map/Reduce and the DFS masters are colocated by default (i.e. run on the same host).

A SOCKS proxy can be configured if you cannot access the Map/Reduce location directly because your machine is not directly connected to the location. See section "How to use SOCKS proxies" for more details. 
