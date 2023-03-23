# CNC Router (BIG WIP)

## Introduction and Safety
The Shapeoko CNC Router is (currently) the most advanced, dangerous, and useful machine that SC Robotics uses. It takes a lot of hours, messed up parts, and broken bits to learn how to use this machine effectively. Don't worry! This documentation page has everything I wish I knew when I first started to use the CNC Router, so you're in good hands as long as you take the time to prepare and learn before jumping in.

The CNC Router is basically a drill that can move around in three axes to drill away material from a stock piece, and turn it into something actually useful.

The CNC Router is also _very_ dangerous. Keep in mind that the spindle is spinning at thousands of RPMs, and cutting metal away like it's butter (if you're using it properly, of course :). There's no need to be scared of it, but keep its dangerous potential in the back of your head and practice these safety precautions:
* Always wear safety glasses. It's not a matter of _if_ something goes flying--they _will_, whether just shavings or broken bits.
* Keep the spindle off unless it's cutting away material. Some people even recomment unplugging it before changing bits.
* _NEVER_ put your hands near an active spindle while the CNC is controlling the stepper motors. If there's something wrong, pause the job, then fix the issue.
    * e.g. the screws on the clamps have become loose form the vibration, and the stock is coming loose. DO NOT tighten the screws while the job is running--pause it first, turn off the spindle, tighten the screws, and resume.
    * e.g. the part is wiggling off of the rest of the stock as the job is almost finished (and you can't add more clamps). DO NOT use your hands to hold it down--use a scrap metal rod to hold it down from a dstance. OR you can use tabs :)
* This goes without saying--follow the `Rules for Machining Success` that will be listed below. Whenever a job isn't going as expected (stock is coming loose, there's bit chatter, bit welding), that's when there's the highest risk of an accident. The best way to prevent accidents is to machine correctly.
* Never leave the CNC Router unattended or attended by someone who doesn't know how it works.
* Use common sense. You'll start to develop a sense for the proper sound and look (even smell, if the bit starts cutting into wood) of a properly-run job. If ANYTHING looks or sounds bad, check the cut and/or stop it.

## Shapeoko Gitbook (MUST READ)
This gitbook covers all of the fundamentals of CNCing with the Shapeoko. You should read through these sections carefully and do further research to make sure you understand these topics:
* Feeds and speeds: feedrate, spindle RPMs, chipload, depth of cut, width of cut, stepover, adaptive tooling, etc.
* Types of bits: flute count, material (e.g. carbide vs HSS?), upcut vs downcut, v-carve, etc.

Outside of that, this book has a lot of good info to just look around.

## CAMing the Part
Might just make a video for this

CAM stands for Computer-Aided Manufacturing. It's how you convert a CAD part into instructions that a machine can understand. Most often, this is in the form of gcode. LINK TO INFO ABOUT GCODE.

Currently, SC Robotics uses Carbide Create to CAM, though there are other popular CAM softwares out there (for the Shapeoko, notably Fusion 360 (which I wanna learn hehe) and MeshCAM). The free version of Carbide Create allows the user to cut strictly 2-D parts, like plates and such. This means the Z-axis never moves at the same time as the X and Y axis. Like a 3D printer, it cuts material away in discrete layers. _Almost all the time, this is all you'll need._ If you need more, it'll require specialized CAM software or outsourcing (or it means you should go change your design because it's too complicated). 

Because everything is 2D, all that Carbide Create needs is a 2D drawing file of the part. This is .DXF file, which you can get from SolidWorks in Save As. 

__EMPIRICAL FEEDS AND SPEEDS TABLE:__

| Bit Diameter | Flute Count | Feed Rate | Spindle RPM | Depth of Cut |
| ------------ | ----------- | --------- | ----------- | ------------ |
| _6061 Aluminum_ |
| 1/16" (112Z) | 2 | 14.0 in/min | 10000 rpm | 0.007" |
| 1/8" (102Z) | 2 | 20.0 in/min | 10000 rpm | 0.010" |
| _Garolite/Fiberglass_ |
| 1/8" (102Z) | 2 | 33.0 in/min | 10000 rpm | 0.025" |


## Setting Up the Stock
Might just make a video for this

At the time of this documentation, there is a 24"x24" section of the bed that is cut away so that it is level with respect to the machine. However, we may soon switch to using purgeable MDF board with large clamps. Anyhow, make sure that your stock lays flat on this section.

Clamp down your stock using tiger-claw clamps to prevent lateral movement. Tiger-claw clamps have two screws--one tightens on the T-Track, and the other pushes horizontally against the stock. Loosen the second, smaller bolt all the way first, and then push the clamp all the way against the stock and tighten both screws. Make sure you have an equal number of tiger-claw clamps on both sides to counteract one force against the other.

Clamp down your stock using the essential T-clamps. These clamps are double-sided--the side with the V-shaped tip is for shorter stock (1/16"~1/4"). The other end is used for thicker stock (>1/2"). These clamps are very important for making sure your Z-axis is accurate because they secure the stock flat against the bed. Make sure there are plenty of these clamps, especially around where your part will be cut.

__NOTE:__ _Do not_ tighten the screws on the clamps too much. They are only there to hold the piece until it's secure enough, and enough that they won't come loose from the CNC vibrations. Tightening too much can strip the screw, damage the T Track, or damage your stock. In the case of the tiger claw clamps, tightening the small screw too much can cause the middle of your stock to bow up (imagine pressing a magazine together from both sides--the middle starts to bend up). In the case of the essential T-clamps, tightening too much can cause warping in the plastic of the clamp, rendering the clamp useless (or less useful at any rate) in the future. For me, this means tightening almost until I can't tighten with the _short_ side of the allen key.

## Setting up the Machine
Might just make a video for this
## Zeroing and Running
Might just make a video for this
## Rules for Machining Success (honestly might be the most important)
* Make sure your workholding is secure before starting to machine!
    * Use tiger claw clamps to prevent lateral movement.
    * Use essential T clamps to keep the workpiece flat against the workbed. This is especially important around the area that you are going to machine the piece, but the whole stock should be clamped.
    * Use your hands to try and move the workpiece--if you can move it, it isn't secure enough.
    * _Remember:_ This is one of the most common mistakes for beginners, so it's important to check this before _every_ job. Any movement of your stock while cutting is not only detrimental to the piece but lends high chances for breaking the very expensive bits.
* Make sure your bit is tightened in the collet. Use both wrenches to tighten for bits 1/4" diameter and bigger
* Z-Axis Leveling
    * Make sure your stock is flat with respect to the CNC. 
    * Zero the Z-Axis near the area your part will be cut. Ensure that this area is sufficiently clamped down. You can even zero the Z-Axis right next to a clamp--just make sure that this clamp is clamping the material above a solid piece of wood, and not above a T channel (if it's clamping above a T channel, the stock material can bend beneath the bed, since there's nothing holding it up)
    * Make sure the actual router is secure in the router holder--if it's loose, the Z-Axis might rise in the middle of a job.
    * _Remember:_ A significant portion of problems that occur with the CNC are due to Z-Axis issues, so following these guidelines is key to successful machining.

_Documented by Micah Hsu_
