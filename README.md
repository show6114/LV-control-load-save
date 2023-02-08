# LabVIEW control value loader and saver

Users can use these VIs to load previously saved control values.

## How to load configuration

![](C:\Users\show6\OneDrive%20-%20TC\LabVIEW%20Dev%202020%2064bit\LV-control-load-save\images\load.png)

Simply wire the `current VI's Path` to the input of the loader. If the configuration file is not existed, this VI create one. 

The configuration file is in `ini` format and save to path `./data/config.ini`. Users can modify the path and file naming for the configuration file in the block diagram. 

Note that the *load* operation is typically run in the early stage of a program. 

## How to save configuration

![](C:\Users\show6\OneDrive%20-%20TC\LabVIEW%20Dev%202020%2064bit\LV-control-load-save\images\save.png)

You do not have to wire anything once the *loader* run. The internal FGV will take over all the stuffs.

Note that the *saver* operation is typically run in the last stage of a program. 
