## Introduction
This documentation isn't a tutorial for how to 3D print--it's mostly a reference page because it's difficult to teach how to use a 3D printer in words. So this assumes you know the basics of using a 3D printer (leveling, printing, etc.)

## Filament
| Material | Heat Deflection | Strength | Ease of Print | Nozzle Temp | Bed Temp | Notes |
| -------- | --------------- | -------- | ------------- | ----------- | -------- | ----- |
| ABS      | High            | Medium   | Hard          | 230-240     | 100-110  | Need enclosure |
| PLA      | Low             | Medium   | Easy          | 200         | 60       |       |
| PLA+     | testing...      | Med/High?| Medium?       | 200?        | 60?      |       |
| TPU      |                 | Compliant| Medium        | ~220        |          |       |
| Onyx     | High            | High     | Easy w/ Glen  | N/A         | N/A      | Glen will help |

## Tolerances
3D Prints are basically melted plastic, so when designing, you need to consider that the plastic will shrink a little bit and add some tolerance.

For clearance holes, to avoid having to drill out the hole, follow this guideline:
* For #10 clearance holes and smaller, the holes should be "Loose" clearance in SolidWorks. 
* For 1/4" clearance holes and larger, they should be "Normal" clearance in SolidWorks.

## Nozzles
You can change the nozzle size to print faster and stronger. Bigger nozzles like 0.8mm nozzles will print much faster and with thicker, stronger layers than a standard 0.4mm nozzle. Smaller nozzles like 0.2mm nozzles will print slower but with more detail.

## Slicing
Slicing is the process of converting a part into layers that a 3D printer can print.

When slicing it's important to remember a few things. First, when saving your part as a .STL from SolidWorks, make sure that the resolution of the file is high enough to create a smooth print. When you File->Save as .STL, click "Options" in the dialog box and make sure the quality is set to "Fine" at minimum.

We use [Ultimaker Cura](https://ultimaker.com/software/ultimaker-cura) to slice our parts, and there are a few key settings to go over:
* Infill: 0-20% for non-structural parts, 20-50% for more structural parts. Anything above roughly 50% and you'll get diminishing returns on strength.
* Infill Pattern: Most common is cubic because it provides a nice multidirection strength-to-weight ratio, but you can also use gyroidal for omnidirectional strength.
* Resolution (Layer Height): For anything that doesn't require detail, print in Draft Quality (max layer height) to print faster. If you need detail, you can decrease the layer height.
* Speed: For PLA and ABS (most common), 50mm/s is standard, but you can safely push up to 65mm/s to save print time. You may want to "Enable Jerk Control" if you do this.
* Support: For any overhanging parts, make sure to turn on supports (duh?) 
* Wall Thickness: sometimes increasing the wall thickness instead of infill will make your print stronger for less filament!

## Misc
You can [iron](https://all3dp.com/2/cura-ironing-3d-printing-ironing/) your 3D prints to create a smooth finish--essentially it runs the hot nozzle over the print without extruding material.

[All3DP](https://all3dp.com/)

_Documented by Micah Hsu_