# 3D Printing Guide

Created by Autumn Painter and Brian Samuel Geyer

## Open 'Cura'
This is where you will adjust the size and orientation of your model for printing. 

First you need to load a .obj file (this is the finished model product). Your model should not have any gaps or holes that could cause issues with printing. 

When you have your object selected, three icons in the bottom left corner will appear: Rotate, Scale, and Mirror

<img src="img/image1.png" width="80%"> 

### Rotate
The bottom left icon is for rotate. The top option allows you to have ‘Cura’ automatically lay your object flat. This will assist in the printing process. You can also manually adjust the orientation of the object with the three adjustment circles that appear. Normally it allows you to adjust in 15 degree increments, but if you press ‘shift’ while rotating, you can rotate at 1 degree increments. 

<img src="img/image2.png" width="40%"> <img src="img/image3.png" width="40%"> 

### Scale
The center bottom icon is for scaling your object. You can either adjust the size of your object based on millimeter measurements or by manualing dragging the scale bar axis (x, y, z) options. You also have the options to have ‘Cura’ scale your object to the largest maximum size to print. 

<img src="img/image4.png" width="40%"> <img src="img/image5.png" width="40%"> 

### Mirror
This option will allow you to automatically flip your object (i.e. mirror) your object along either the X, Y, or Z axis. 

<img src="img/image6.png" width="20%"> 

## Adjusting the Print File
Within the toolbox on the left side of the screen, you are able to adjust many different options that will affect the print quality, fill, speed, and temperature. 

<img src="img/image7.png" width="40%"> <img src="img/image8.png" width="40%"> 

### Quality:

#### Layer Height (mm)
This is the most important setting for determining the quality of your print. Normal quality prints are 0.1 mm, high quality prints are 0.06 mm. You can go up to 0.25 mm with the Ultimaker for a very fast print at a very low quality.

Note: some guides or publications report layer heights in microns. 1 mm is 1000 microns, so 0.1 mm is 100 microns and 0.06 mm is 60 microns. Ultimaker claims that our printer, using the 0.4 mm nozzle we leave installed in our printer, can achieve a 20-micron layer height resolution. For more information, see [Ultimaker's specifications for their 2+ line](https://web.archive.org/web/20190605134603/https://ultimaker.com/en/products/ultimaker-2-plus/specifications). For information about other Ultimaker printers, you can also look at their [printer-specific documentation](https://support.ultimaker.com/hc/en-us/categories/360002327580-3D-Printers).

#### Shell Thickness (mm)
This thickness is of the outside shell in the horizontal direction. This is used in combination with the nozzle size to define the number of perimeter lines and the thickness of those perimeter lines. 

#### Enable Retraction
This allows for the filament to be retracted when the nozzle is moving over a ‘none-printed’ area. More details about the retraction can be configured in the advanced tab. 

### Fill:

#### Bottom/Top Thickness (mm)
This controls the thickness of the bottom and top layers, the amount of solid layers put down is calculated by the layer thickness and this value. Having a value a multiple of the layer thickness make sense. And keep it near your wall thickness to make an evenly strong part.

#### Fill Density (%)
This controls how densely filled the insides of your print will be. For a solid part use 100%, for an empty part use 0%. A value around 20% is usually enough. This will not affect the outside of the print and only adjusts how strong the part becomes. 

### Speed and Temperature:

#### Print speed (mm/s):
Speed at which the printing happens. A well adjusted Ultimaker can reach 150mm/s, but for a good quality print, you want it to print slower. Printing speed depends on a lot of factors. So this is one setting that you will experiment with. 

### Support:

#### Support type
This is where you choose between no support type, support through touching the buildplate, or an ‘everywhere’ support type. Touching buildplate only creates support where the support structure will touch the build platform; everywhere support creates support even on top of parts of the model.

#### Platform adhesion type
This is where you will choose between no platform adhesion, a brim platform adhesion, or a raft adhesion. Each of these are different options which help in preventing corners from lifting due to warping. Brim adds a single layer thick flat area around your object which is easy to cut off afterwards, and it is the recommended option. Raft adds a thick raster below the object and a thin interface between this and your object. 

## View Mode
You are able to view your model in a variety of ways including: normal, overhang, transparent, x-ray, and layers. To switch between these options click the icon located in the top right corner of the of the program (see image). 

<img src="img/image9.png" width="20%"> 

## Save Model
To save your model you can either go to File → Save GCode, or you can click the floppy disk save icon (Save toolpath option) in the top left corner of the screen (see image below). If you have the SD card plugged into the computer, the ‘save toolpath’ option will automatically save the model to that location.

<img src="img/image10.png" width="80%"> 

## How to Print on Ultimaker:
NOTE: These instructions are written for explaining an Ultimaker 2+ Extended. These instructions should generally apply to other printers as well - especially other Ultimaker models - but the links are mostly to pages with Ultimaker-provided instructions for the 2, 2+, and/or 2+ Extended. For other Ultimaker printers, check the [specific model's documentation](https://support.ultimaker.com/hc/en-us/categories/360002327580-3D-Printers).

### Printing:
1. Plug SD card with .gcode file of the object
1. Turn on Ulitmaker printer. Switch is on the back left corner.
1. Confirm that filament is inserted into the printer.
1. If you want to use glue on the glass plate, do that now.
1. To print, scroll using the round controller to the print option and press the controller. This will open a new screen that will list the .gcode files. Your most recent file will most likely be at the end of the list.

NOTE: It is possible to remove or add the SD card while the printer is on, as long as it isn't currently trying to access that card, such as by being currently printed or displaying the SD card contents. 

#### Printer Display and Controller:
[https://support.ultimaker.com/hc/en-us/articles/360011888779-Display-and-controller-on-the-Ultimaker-2-](https://support.ultimaker.com/hc/en-us/articles/360011888779-Display-and-controller-on-the-Ultimaker-2-)

#### Inserting New Filament Material:
[https://support.ultimaker.com/hc/en-us/articles/360012004880-How-to-insert-filament](https://support.ultimaker.com/hc/en-us/articles/360012004880-How-to-insert-filament)

#### Changing Filament:
[https://support.ultimaker.com/hc/en-us/articles/360011848000-Changing-filament-of-the-Ultimaker-2](https://support.ultimaker.com/hc/en-us/articles/360011848000-Changing-filament-of-the-Ultimaker-2)

#### Using Glue:
[https://support.ultimaker.com/hc/en-us/articles/360011953459-Using-glue-on-the-Ultimaker-2](https://support.ultimaker.com/hc/en-us/articles/360011953459-Using-glue-on-the-Ultimaker-2)

#### Calibrating the Printer:
[https://support.ultimaker.com/hc/en-us/articles/360011801020-Build-plate-calibration-for-the-Ultimaker-2-](https://support.ultimaker.com/hc/en-us/articles/360011801020-Build-plate-calibration-for-the-Ultimaker-2-)

### Maintenance:

#### Cleaning the Glass Plate:
[https://support.ultimaker.com/hc/en-us/articles/360011953699-Cleaning-the-glass-plate-of-the-Ultimaker-2](https://support.ultimaker.com/hc/en-us/articles/360011953699-Cleaning-the-glass-plate-of-the-Ultimaker-2)

#### The Feeder:
[https://support.ultimaker.com/hc/en-us/articles/360011848300-The-Ultimaker-2-feeder](https://support.ultimaker.com/hc/en-us/articles/360011848300-The-Ultimaker-2-feeder)

#### Lubricating the Axles:
[https://support.ultimaker.com/hc/en-us/articles/360011848520-Lubricating-the-Ultimaker-2-axles](https://support.ultimaker.com/hc/en-us/articles/360011848520-Lubricating-the-Ultimaker-2-axles)

#### Unclogging Nozzle- Atomic Method:
[https://support.ultimaker.com/hc/en-us/articles/360011954019-Atomic-method-for-the-Ultimaker-2](https://support.ultimaker.com/hc/en-us/articles/360011954019-Atomic-method-for-the-Ultimaker-2)

### Troubleshooting:

#### Extrusion Problems:
[https://support.ultimaker.com/hc/en-us/articles/360011848800-Extrusion-problems-on-the-Ultimaker-2](https://support.ultimaker.com/hc/en-us/articles/360011848800-Extrusion-problems-on-the-Ultimaker-2)

#### Error Messages:

##### Original Ultimaker Original
[https://support.ultimaker.com/hc/en-us/articles/360012040879-Error-messages-for-the-Ultimaker-Original](https://support.ultimaker.com/hc/en-us/articles/360012040879-Error-messages-for-the-Ultimaker-Original)

##### Ultimaker Original+
[https://support.ultimaker.com/hc/en-us/articles/360011910820-Error-messages-for-the-Ultimaker-Original-](https://support.ultimaker.com/hc/en-us/articles/360011910820-Error-messages-for-the-Ultimaker-Original-)

##### Ultimaker 2
[https://support.ultimaker.com/hc/en-us/articles/360011849380-Error-messages-for-the-Ultimaker-2](https://support.ultimaker.com/hc/en-us/articles/360011849380-Error-messages-for-the-Ultimaker-2)

##### Ultimaker 2 Extended
[https://support.ultimaker.com/hc/en-us/articles/360011984099-Error-messages-for-the-Ultimaker-2-Extended](https://support.ultimaker.com/hc/en-us/articles/360011984099-Error-messages-for-the-Ultimaker-2-Extended)

##### Ultimaker 2+
[https://support.ultimaker.com/hc/en-us/sections/360003497520-Error-messages](https://support.ultimaker.com/hc/en-us/sections/360003497520-Error-messages)

##### Ultimaker 2 Go
[https://support.ultimaker.com/hc/en-us/articles/360011830280-Error-messages-for-the-Ultimaker-2-Go](https://support.ultimaker.com/hc/en-us/articles/360011830280-Error-messages-for-the-Ultimaker-2-Go)

##### Ultimaker 2 Connect
[https://support.ultimaker.com/hc/en-us/sections/360004445680-Error-messages](https://support.ultimaker.com/hc/en-us/sections/360004445680-Error-messages)

##### Ultimaker 3
[https://support.ultimaker.com/hc/en-us/sections/360003523739-Error-Messages](https://support.ultimaker.com/hc/en-us/sections/360003523739-Error-Messages)

##### Ultimaker S5
[https://support.ultimaker.com/hc/en-us/sections/360003524399-Error-messages](https://support.ultimaker.com/hc/en-us/sections/360003524399-Error-messages)

#### Can’t Update Firmware:

##### Ultimaker Original
[https://support.ultimaker.com/hc/en-us/articles/360011939420-Can-t-update-the-Ultimaker-Original-firmware](https://support.ultimaker.com/hc/en-us/articles/360011939420-Can-t-update-the-Ultimaker-Original-firmware)

##### Ultimaker Original+
[https://support.ultimaker.com/hc/en-us/articles/360012014819-Can-t-update-the-Ultimaker-Original-firmware](https://support.ultimaker.com/hc/en-us/articles/360012014819-Can-t-update-the-Ultimaker-Original-firmware)

##### Ultimaker 2
[https://support.ultimaker.com/hc/en-us/articles/360011849580-Can-t-update-the-Ultimaker-2-firmware](https://support.ultimaker.com/hc/en-us/articles/360011849580-Can-t-update-the-Ultimaker-2-firmware)

##### Ultimaker 2 Extended
[https://support.ultimaker.com/hc/en-us/articles/360011984299-Can-t-update-the-Ultimaker-2-Extended-firmware](https://support.ultimaker.com/hc/en-us/articles/360011984299-Can-t-update-the-Ultimaker-2-Extended-firmware)

##### Ultimaker 2 Go
[https://support.ultimaker.com/hc/en-us/articles/360011933899-Can-t-update-the-Ultimaker-2-Go-firmware](https://support.ultimaker.com/hc/en-us/articles/360011933899-Can-t-update-the-Ultimaker-2-Go-firmware)

#### Print not sticking to build plate:
[https://support.ultimaker.com/hc/en-us/articles/360011954939-Print-not-sticking-to-the-Ultimaker-2-build-plate](https://support.ultimaker.com/hc/en-us/articles/360011954939-Print-not-sticking-to-the-Ultimaker-2-build-plate)

## Common Issues and Adjustment Suggestions:

### Raft vs. No Raft vs. Brim? 
An issue that can arise when printing 3D models. How secure of a base does the model need? Depending on this, you can decide which base to print. If the print needs a lot of security/stability, choose the raft option. Additionally, a raft can make up for any unevenness in the buildplate’s level, however rafts use quite a bit of extra material. A good alternative to try first is a brim, especially for well-calibrated printers, which is a balance between extra stability without too much extra material being used.

Jammed nozzle →  Refer to the Atomic Method

-----
### Return to [LEADR's Resources list](https://leadr-msu.github.io/)
