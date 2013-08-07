CityGen Maya Script

CityGen is a procedural cityscape generator for Maya written in python. This can be done through either procedurally created buildings, or with user-supplied buildings. 

Using CityGen

First, install the CityGen script by copying the cityGen.py file to your scripts folder.
In Mac OS X, this is located at /Users/[username]/Library/Preferences/autodesk/maya/scripts
In Windows, this is located at c:/Users/[username]/Documents/maya/2013-x64/scripts/

Note: Depending on your OS and Maya version, these paths may differ

2.   Once you've installed the script, open up the script editor
3.   Copy and paste the following code into the editor. Once you've done that, highlight the code and drag and drop it onto your custom shelf to add it to your shelf.


import maya.cmds as cmds
import cityGen as cg
reload(cg)
cg.UI()


4.   Press the newly created button to run the GUI.
5.   Below are the options available to you in the GUI
City Width: The width of the city
City depth: The depth of the city
Maximum Building Height: when using the procedural buildings, this controls how tall they can be
Building Gap: The space between buildings
Street Width: How wide the streets are
Block Size: The width of a city block, or the distance between streets

6.   Procedural Buildings vs. User Created
If you'd like to have the script create a set of sample buildings for you, simply run the script without anything being selected
To have the script replicate buildings that you've created, first group the buildings so they're under a single group node. Select the group node, and then press the generate button

Note: Be careful when using user generated buildings. If your buildings have a high polycount and you're creating a large city, you could run into memory issues.