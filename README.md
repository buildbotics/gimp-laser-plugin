# gimp-laser-plugin
A plugin for Gimp which turns images into GCode for LASERS

# Installation
Start by opening gimp to find. From within gimp, select Edit->Preferences.
Then, expand Folders in the lefthand pane. Then, select Plugins. This will show
places where gimp looks for plugins.

## linux installation
Drop 'BUILDBOTICS-laser-plugin' into the folder found above.

## Windows 10 installation
For Gimp 2.10, Drop 'BUILDBOTICS-laser-plugin-for-gimp2.10.py' into 
the folder found above.

For Gimp 2.8, Drop 'BUILDBOTICS-laser-plugin-for-gimp2.8.py' into
the folder found above.
 
# Running the plugin
Then select ``File -> Export g-code for laser engraving..`` to run the plug-in.
The plugin will be "grayed out" and inaccessible until an image is loaded.

After loading and image and making any desired changes, select
'File->Export g-code for laser engraving' to open the plugin.
