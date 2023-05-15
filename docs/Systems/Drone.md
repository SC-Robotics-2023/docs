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