# Hardware
Overview of the most common hardware on the rover!
## Fasteners
### Bolts
> __Bolts__ are fasteners with externally threaded shafts. They fasten onto a nut or female-threaded hole. Bolts we use are typically tightened with a hexagonally-shaped key. 

In this image, a bolt mates with a __nut__ on the opposite side of the material to be fastened:  
![Bolt and Nut](./img/Bolt%20and%20Nut.png)

In this image, a bolt goes through a __clearance hole__ (a hole that the bolt slips through) on one plate and mates with a __tapped hole__ (a hole that has threads in it) on a second plate:  
![Bolt and Tapped Hole](./img/Bolt%20and%20Tapped%20Hole.png)

There are several important characteristics of bolts, including the system of measurement, naming, and head type.
* Metric vs Imperial: metric bolts use mm for dimensions, while imperial bolts use in for dimensions.
* Bolt sizing
    * Metric: `nominal diameter`-`pitch` x `length`.
        * e.g. M4-0.7 x 12 is a bolt with a 4mm diameter, 0.7mm between threads, and 12mm of length
    * :star:Imperial: `major diameter`-`threads per inch` x `length`
        * e.g. 1/4-20 x 1/2" is a bolt with 1/4" diameter, 20 threads per inch, and 1/2" of length
    * As you work, you will begin to memorize these useful dimensions for imperial bolts:

![Imperial Drill and Tap Chart](./img/Imperial%20Chart.png)

:::tip
Use imperial first. Only use metric if off-the-shelf items require them. The most common bolts we use are #10 and 1/4" bolts--these should cover 90% of your needs.
:::

* Head Types:
    * :star:Button Head: Used for standard load applications.
    * Socket Head: Used for high load applications. Taller head and bigger hex size allows for more torque to be applied when tightening, but requires more clearance.
    * Flat Head (CounterSunk): Used when little clearance is available for a head. Requires countersink drill bit.

![Bolt Types](./img/Bolt%20Types.png)

* Loctite
    * Loctite threadlocker is a liquid or gluestick that you rub on _the first few_ threads of the bolt before fastening onto a tapped hole (not on nuts). It then expands and solidifies to fill the gap between the threads, friction-locking the bolt in place.
    * You should always use loctite on final assembly because screws can loosen and fall out due to vibration.
    * When adding loctite, clean off any old loctite (white crust) before reapplying to ensure the new loctite has clean threads to tighten.
    * In almost all cases, _use blue loctite_.

![Loctite](./img/Loctite.png)

:::caution
Do not use loctite for any bolt that fastens through plastic--the fumes released may crack/weaken the plastic. Use super glue instead if necessary.
:::

<details>
<summary>Advanced Topics</summary>
<ul>
    <li>Coarse threads vs fine threads: In the imperial system, every bolt diameter has a coarse and a fine threaded version (UNC vs UNF) that indicates the relative threads per inch</li>
        <ul>
            <li>For example, a #10 bolt has 10-24 (coarse) and 10-32 (fine) threading.</li>
            <li>Fine threads are more likely to be <a href="https://pedalchile.com/blog/cross-threading">galled/cross-threaded</a> and require more turns to fasten, but are stronger overall because there are more threads.</li>
            <li><a href="https://www.nord-lock.com/insights/bolting-tips/2010/choose-fine-or-coarse-thread-bolts/">Pros and Cons</a></li>
        </ul>
    <li>Imperial bolt size numbers follow this equation: 0.06" + (0.013 x number)</li>
</ul>
</details>

### Nuts
> __Nuts__ are fastening elements used in conjunction with screws.

There are many different types of nuts for different applications. Some of these are listed:
* Hex Nuts: general purpose nut
* :star:Lock Nuts: a nylon insert compresses when the bolt is fastened, "locking" the nut in place. _most commonly used_
* Flange Nuts: a flange distributes pressure, so you don't need a washer
* Wing Nuts: wings allow tightening and loosening by hand

![Types of Nuts](./img/Types%20of%20Nuts.png)

### Rivets
> __Rivets__ are permanent fasteners that work by squeezing two items teogether by forcefully crushing metal. They are used when you can only access one side of the material, and are very easy to use with the right tools.

![Rivet Animation](./img/Rivet%20Animation.gif)  
There are a couple important parts of a rivet:
* Rivet pin: important features are diameter and grip length. Grip length determines how thick the material that you are fastening together can be.
* Head: the head can be dome-headed (similar to button-headed bolts) or flush-headed (similar to flat-headed bolts)

![Rivet Diagram](./img/Rivet%20Diagram.png)  
:::note
Rivets aren't fully permanent--they can be "drilled out" and replaced using a drill bit that corresponds to the diameter of the rivet pin

The most common rivet we use is a 3/16" diameter rivet that fits into a 0.196" hole (hole size for #10 clearance). The hole is bigger because the rivet expands. 
:::

### Washers
> __Washers__ are used to distribute the load of tightening a bolt over a wider area, allowing the bolt to be more strongly tightened without damage to the surface. Especially important for plastic.  

There are many different kinds of washers that you can look up for more info--some are shown in the image below:  
![Washers](./img/Washers.png)

:::note
Flat washers, the most common washer, have a flat side and a rounded side--the flat side goes to the material and the rounded side goes to the bolt
:::

## Rotary Motion
### Shafts and Spacers
> __Shafts__ are used everywhere for rotary transmission. The most common for our use are __roundshafts__ and __hex shafts__.
>> __Spacers__ are just cylinders that keep distance between two elements on a shaft. They're typically nylon plastic.

![Hex Shaft](./img/Hex%20Shaft.png)
![Round Shaft](./img/Round%20Shaft.png)
![Thunderhex Shaft](./img/Thunderhex%20Shaft.png)

### Gears
> __Gears__ are one of the most basic pieces of rotary transmission hardware. They are used to swap rotation direction and in gearboxes for reducing speed/increasing torque.

There are a few important characteristics about gears:
* Tooth Count: How many teeth there are, needed for gear ratios.
* Pitch Diameter: Important for designing gears to mesh. Essentially, if the pitch diameters of two gears are tangent to one another, then the gears will mesh properly.
* Outer Diameter: The diameter of the whole gear.
* Center Distance: The distance between the centers of the gears.

![Spur Gear](./img/Spur%20Gear.png)

:::tip
Avoid brass gears--they'll get chewed up. Use 7075 aluminum or steel gears.
:::

<details>
<summary>Advanced Topics</summary>
Another important feature of gears is Diametral Pitch (DP), which is the ratio of the number of teeth to the pitch diameter--higher DP allows you to fit gears in tight spots.
<br></br><br></br>
Technically, the gear shown in the picture above is a <strong>spur gear</strong>. However, there are many other useful types of gears:
<ul>
    <li><a href="https://en.wikipedia.org/wiki/Bevel_gear">Bevel Gears</a>: Used for 90 deree rotational transmission. A bevel gear with a 1:1 ratio is called a <strong>miter gear</strong>.</li>
    <li><a href="https://www.iqsdirectory.com/articles/gear/worm-gears.html">Worm Gears</a>: While <strong>spur gears</strong> can cause a lot of <a href="https://en.wikipedia.org/wiki/Backlash_(engineering)">backlash</a>, worm gears are great for reducing backlash and smooth motion, as well as big gear reductions and quieter operation.</li>
    <li><a href="https://en.wikipedia.org/wiki/Rack_and_pinion">Gear Racks (aka Rack and Pinion)</a>: Simple mechanism used to convert rotational motion to linear motion via gears.</li>
    <li><a href="https://www.differencebox.com/engineering/difference-between-helical-gear-and-herringbone-gear/">Helix and Herringbone Gears</a>: <strong>Helical gears</strong> have teeth angled in a helix, resulting in more teeth contact and stronger power transmission, with side effect of some axial thrust force. <strong>Herringbone</strong> gears also have angled teeth, but they are shaped like a V so that the axial thrust forces cancel each other out. A Herringbone gear is a solid choice for 3D printed gears, as it gives more tooth contact and is quieter.</li>
</ul>
</details>

### Bearings and Bushings
> __Bearings__ are commonly used to minimize the friction of a spinning shaft. An important feature of both bearings and bushing is whether or not they are __flanged__.

There are several different kinds of bearings that we've used commonly:  
* Ball Bearings
    * The shaft that spins goes in the middle and turns with the inner race.
    * There are two important kinds of bearings: radial and flanged. Radial bearings have no flange and slip through holes. Flanged bearings have a flange on the outside so they can rest on a surface. 

![Ball Bearing](./img/Ball%20Bearing.png)
![Flanged Bearing](./img/Flanged%20Bearing.png)
![Ball Bearing Diagram](./img/Ball%20Bearing%20Diagram.png)

> __Bushings__ are similarly used to minimize friction but have no moving elements and are _used for low speeds of rotation_. They are simply a low-friction cylinder made by injecting lubricant into metal somehow.

![Bushing](./img/Bushing.png)

<details>
<summary>Advanced Topics</summary>
There are a couple more kinds of useful bearings that we have used: 
<ul>
    <li><a src="https://www.ritbearing.com/blog/archive/what-are-needle-roller-bearings/">Needle Roller Bearings</a>: Used where the shaft is too large and a ball bearing would get too big.</li>
    <li><a src="https://tameson.com/pages/thrust-bearings">Thrust Bearings</a>: Used where two faces rotate against each other and support axial loads.</li>
</ul>
</details>

### Lead Screws
> __Lead screws__ are essentially long bolts that are used to convert rotational motion to linear motion.

![Lead Screw Animation](./img/Lead%20Screw.gif)

<details>
<summary>Advanced topics</summary>

(click links on certain key words for more info)

Some lead screws are [__back-driveable__](https://www.pbclinear.com/Blog/2018/February/What-is-Lead-Screw-Efficiency-in-Linear-Motion#:~:text=What%20is%20Back%20Driving%3F), i.e. when a linear force is applied, the nut will turn and move backwards. Other lead screws are not back-driveable because the friction force increases faster than the torque to turn. Because a lead screw is essentially an inclined plane, back-driveability is analagous to the [__angle of repose__](https://en.wikipedia.org/wiki/Angle_of_repose#:~:text=This%20free%20body%20diagram%20demonstrates%20the%20relationship%20between%20angle%20of%20repose%20and%20material%20on%20the%20slope.) of an object on an inclined plane. Back-driveability is related to the [__helix and lead angle__](https://fractory.com/lead-screws/#:~:text=Helix%20and%20lead%20angle) as well as the [__efficiency__](https://www.helixlinear.com/blog/lead-screws/lead-screws-vs-ball-screws-which-will-work-best-for-your-application/#:~:text=Efficiency%20in%20linear,the%20screw%20thread.) of the lead screw because efficiency is related to losses of friction.

Lead screws have several different types of [__thread profiles__](https://fractory.com/lead-screws/#:~:text=obtain%20the%20lead.-,Types%20of%20Lead%20Screw%20Threads,-Lead%20screws%20are), and these affect strength, precision, and back-driveability.

Lead screws can have more than one [__start__](https://www.thomsonlinear.com/en/support/tips/difference-between-screw-pitch-and-lead), meaning there are multiple individual threads running along the length of the shaft. More starts means more __lead distance__ (distance traveled/revolution).

[__Ball screws__](http://www.barnesballscrew.com/how-a-ball-screw-works/) are an alternative to lead screws that use actual balls (similar to ball bearings) to travel, decreasing friction and increasing back-driveability.
</details>

### Retaining Rings and Shaft Collars
> __Retaining rings__ are a low-profile solution put on the end of a shaft to stop the shaft from falling out the other way.

There are two most common kinds of retaining rings: snap rings and e-clips. They fit into a groove on the shaft of specified width and diameter.

![Retaining Rings](./img/Retaining%20Rings.png)

> __Shaft Collars__ are a high-profile and strong clamp to stop the shaft from falling out. They commonly use bolts or __set screws__ (a fully threaded screw with no head cap) to clamp.

![Clamping Shaft Collar](./img/Clamping%20Shaft%20Collar.png)
![Set Screw Collar](./img/Set%20Screw%20Collar.png)

## Examples on the Rover!
_Documented by Micah Hsu_