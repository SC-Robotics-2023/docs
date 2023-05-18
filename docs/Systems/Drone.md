# Drone Documentation

## Preliminary Research and Design Constraints
* Design Constraints
    * _Flight Time:_ For full autonomy mission, must operate for ~>30 mins. For part autonomy mission, must operate for <30 mins.
    * _Navigation Capability:_ Must fly below 400 feet above ground level. Must operate in 40 kph/30 mph wind, which means a top speed of at least 64 kph/40 mph.
    * _Mass Constraints:_ Must not exceed 5 kg. Must carry inert dummy mass of the same weight as the battery (in winds <= 24 kph/15 mph winds)
    * _Autonomous Capability:_ Same as rover
    * Must meet FAA guidelines
* Overall Design
    * Quadcopter
        * Pros:
            * Very well documented as a hobby project
            * Simple
            * Hover capable
        * Cons:
            * Battery inefficiency
    * Fixed Wing
        * Pros:
            * Battery efficiency
        * Cons:
            * Hover incapable
    * Mixed Mode
        * Pros:
            * Battery efficiency
            * Hover capable
        * Cons:
            * Complexity in design, analysis, and prototyping
* Potentially Helpful Sofware
    * [XFLR5](http://www.xflr5.tech/xflr5.htm) - Analysis for airfoilds, wings, etc.
    * [OpenVSP](https://openvsp.org/) - NASA parametric geometry
    * [ANSYS](https://www.ansys.com/) - Industry simulation software, CFD
    * [eCalc](https://www.ecalc.ch/) - Electric drive simulator for motor calculations
    * [ArduPilot Mission Planner](https://ardupilot.org/planner/) - Mission routing/planning
    * [Pixhawk](https://pixhawk.org/) - Drone hardware standards  
* Electrical Hardware
    * 6 DOF IMU
    * 1D LiDAR
    * Camera
    * GPS with Magnetometer
    * [Cube Orange Flight Controller](https://docs.px4.io/main/en/flight_controller/cubepilot_cube_orange.html)
    * [RFD900 RC Transmitter Module](https://store.rfdesign.com.au/rfd900-txmod-v2-rc-transmitter-module/)
* Design Material
    * Carbon Fiber Nylon 3D Printing
        * Research Vacuum Bagging

## Quadcopter Design
* Physics behind Quadcopters
    * Four propellers, two rotate clockwise, two rotate counterclockwise.
    * Vertical, lateral, and rotational movement
    * [The Science Behind Quadcopters](https://www.nasa.gov/sites/default/files/atoms/files/aam-science-behind-quadcopters-reader-student-guide_0.pdf)
* Propeller Blades
    * L x P x B - Length x Pitch x Blades
    * Length: Smaller blades are for smaller payloads and motors with high kV, vise versa. Larger blades produce more stability while flying in the air.
    * Pitch: Lower pitch moves faster, draws less current, and produces less turbulence, but produces less thrust, vise versa. There are fixed and variable pitch propellers, but variable pitch propellers are much more complex.
    * Blades: Fewer blades draws less current but produces less thrust and less control. 3 is a safe middle ground between high speed vs control, for 3-7" aircraft.
    * Thrust Calculations:
        * Thrust-to-weight ratios (TWR) (from [calctool](https://www.calctool.org/machines-and-mechanisms/drone-motor#thrust-to-weight-ratio)):

            | Application | Thrust-to-Weight Ratio |
            | ----------- | ---------------------- |
            | Aerial Photography | 2:1 |
            | FPV Video | 4:1 |
            | Drone Races | 5:1 |
            | Acrobatic Flying | 7:1 |
            * Suppose we desire a 2:1 TWR. In the worst case, the drone will weight 5 kg, so the required thrust will be 10 kg. Since there are four propellers, each propeller/motor will have to produce an overall thrust of 2.5 kg
            * A TWR of 2:1 is a [good number to aim for](https://www.youtube.com/watch?v=KgTN_VuKORs) for most normal drones that won't be flying fast. Based on this, we should __aim for a TWR between 2:1 and 3:1__
        * [To calculate](https://www.tytorobotics.com/blogs/articles/how-to-calculate-propeller-thrust) the required features to produce a certain thrust, we can use a [thrust calculator](https://www.mejzlik.eu/technical-data/propeller_calculator). Static vs Dyanimic Thrust
    * Top Speed
        * Theoretical top speed can be calculated [via the equation](https://oscarliang.com/propellers/#What-Propellers-To-Use-on-an-FPV-Drone:~:text=Max%20Speed%20(in%20inch%20per%20second)%20%3D%20Max%20RPM%20*%20Propeller%27s%20Pitch%20/%2060) `Max Speed (in inch per second) = Max RPM * Propeller's Pitch / 60`, but this does not incorporate air resistance, head wind, or angle of attack.
* Drone Size Class
    * 6 inch and 7 inch drones can carry more payload and are ideal for long range flight. The expense is that they aren't as agile, but that doesn't really matter for our purposes. __7 inch drone class is probably the way to go.__
* Motors
    * Motors correspond to the drone size and more particularly, the propeller size. Suggestions [here](https://oscarliang.com/motors/#Brushless-vs-Brushed-Motors:~:text=For%20a%20more%20detailed%20table%20encompassing%20various%20prop%20sizes%20and%20LiPo%20voltages%2C%20check) and [here](https://fpv-shopping-list.com/top-3-mistakes-with-7-inch-drones). Aim for 1200KV motors of size 2507-2508.
* Battery
    * There are two main types of batteries: 4S and 6S LiPO batteries. 6S LiPO batteries boast longer flight time, lower current draw, and longevity, but at a higher cost and weight.
    * Capacity and charge rate.
### Component Selection
* Propellers
    * [HQProp DP 7X4X3 Propeller](https://www.getfpv.com/hqprop-dp-7x4x3-propeller-set-of-4-light-grey.html). Seen this propeller recommended on multiple builds and websites.
        * Size: 7"
        * Pitch: 4"
        * Material: PC
        * Blades: 3
        * Weight: 9.27g
        * Mounting hole: 5mm
        * Center Hub Thickness: 7mm
        * POPO Compatible: Yes
* Motors
    * [Avenger V2](https://www.brotherhobbystore.com/avenger-2507-v2-motor-p0082-p0082.html)
* Battery
    * Need to do battery calculations

## Mixed Mode Design

