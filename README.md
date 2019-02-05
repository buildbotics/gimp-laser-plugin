# gimp-laser-plugin
A plugin for Gimp which turns images into GCode for LASERS

# Installation
Start by opening gimp. From within gimp, select Edit->Preferences.
Then, expand Folders in the lefthand pane. Then, select Plugins. This will show
where gimp looks for plugins.

## linux installation
Drop 'BUILDBOTICS-laser-plugin' into the folder found above.

## Windows 10 installation
For Gimp 2.10, Drop 'BUILDBOTICS-laser-plugin-for-gimp2.10.py' into 
the folder found above.

For Gimp 2.8, Drop 'BUILDBOTICS-laser-plugin-for-gimp2.8.py' into
the folder found above.
 
# Running the plugin
Then select ``File -> Export g-code for laser engraving...`` to run the plug-in.
The plugin will be "grayed out" and inaccessible until an image is loaded.

After loading and image and making any desired changes, select
'File->Export g-code for laser engraving' to open the plugin.

<img src="images/plugin.png" width="40%">

All distance values are entered in millimeters.

The "Output image width (mm)" field specifies how wide the resulting LASER image will be.

The "Size of one output pixel (mm)" specifies the size of a single pixel. For instance, a
value of .25 means each pixel in the LASER image will be .25mm square.

"Feed rate in mm/minute" specifies the rate at which the LASER head will move relative to the surface work
piece while the LASER is on.

"Minimum LASER S-value" specifies the power setting for the LASER at its lowest power.

"Maximum LASER S-value" specifies the power setting for the LASER at its highest power.

"Minimum rapid distance movement" specifies the minimum distance that will be converted to a
rapid move when the LASER is off. For instance if the LASER output is at zero and a move of 20 millimeters
is encountered, that move would be converted to a rapid move if the setting is set to 10, but would not be
converted to a rapid move if the setting is set to 25.

"Minimum pixel value" sets the minimum pixel value that will result in turning on the LASER.
For instance, if this field is set to 20, pixels with a value less than 20 will result in the LASER
power being set to 0.

"Laser intensity (%)" scales the output LASER power by the amount specified. Lower settings
result in lighter engraved images.

Clicking "OK" causes the user to be prompted for an output file and folder. Then the resulting g-code
is created and saved in the file that was specified.
