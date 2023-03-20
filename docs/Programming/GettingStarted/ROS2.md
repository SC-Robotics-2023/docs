# ROS2

## What is ROS2?
- The Robot Operating System (ROS) is a set of software libraries and tools for building robot applications. From drivers and state-of-the-art algorithms to powerful developer tools, ROS has the open source tools you need for your next robotics project.
- It is used to communicate between different parts of any systems, by wrapping the data in a standard format and sending it over a network.
- It is also used to create a system that can be easily extended and modified.
- If you have Ubuntu 20.04 LTS, you can install ROS2 [here](https://docs.ros.org/en/foxy/index.html)
- If you have Ubuntu 22.04 LTS, you can install ROS2 [here](https://docs.ros.org/en/humble/index.html)

-----------------------------------------

## ROS2 concepts and why we use them
- I would suggest you walk through the following tutorials to get a better understanding of ROS2 concepts and why we use them. I feel like its better to read and learn from the source rather than me explaining it here.
- Though if you have a hard time understanding the tutorials, feel free to ask me any questions you have. And its totally fine if you don't get it the first time, I'd dive into our `2022-23 Drive code` to get a better understanding of how we use ROS2. There we used the simplest form of ROS2, which is the `Publisher-Subscriber` architecture.
- Beginner: CLI tools
    + [Configuring environment](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Configuring-ROS2-Environment.html)
    + [Understanding nodes](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Understanding-ROS2-Nodes/Understanding-ROS2-Nodes.html)
    + [Understanding topics](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Understanding-ROS2-Topics/Understanding-ROS2-Topics.html)
    + [Understanding services](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Understanding-ROS2-Services/Understanding-ROS2-Services.html)
    + [Understanding parameters](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Understanding-ROS2-Parameters/Understanding-ROS2-Parameters.html)
    + [Understanding actions](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Understanding-ROS2-Actions/Understanding-ROS2-Actions.html)
    + [Launching nodes](https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Launching-Multiple-Nodes/Launching-Multiple-Nodes.html)

- Beginner: Client libraries
    + [Using colcon to build packages](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Colcon-Tutorial.html)
    + [Creating a workspace](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Creating-A-Workspace/Creating-A-Workspace.html)
    + [Creating a package](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html)
    + [Writing a simple publisher and subscriber (C++)](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Cpp-Publisher-And-Subscriber.html)
    + [Writing a simple publisher and subscriber (Python)](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Py-Publisher-And-Subscriber.html)
    + [Writing a simple service and client (C++)](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Cpp-Service-And-Client.html)
    + [Writing a simple service and client (Python)](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Py-Service-And-Client.html)
    + [Creating custom msg and srv files](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Custom-ROS2-Interfaces.html)
    + [Implementing custom interfaces](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Single-Package-Define-And-Use-Interface.html)
    + [Using parameters in a class (C++)](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Using-Parameters-In-A-Class-CPP.html)
    + [Using parameters in a class (Python)](https://docs.ros.org/en/foxy/Tutorials/Beginner-Client-Libraries/Using-Parameters-In-A-Class-Python.html)

- Intermediate
    + [Managing Dependencies with rosdep](https://docs.ros.org/en/foxy/Tutorials/Intermediate/Rosdep.html)
    + [Creating an action](https://docs.ros.org/en/foxy/Tutorials/Intermediate/Creating-an-Action.html)
    + [Writing an action server and client (C++)](https://docs.ros.org/en/foxy/Tutorials/Intermediate/Writing-an-Action-Server-Client/Cpp.html)
    + [Writing an action server and client (Python)](https://docs.ros.org/en/foxy/Tutorials/Intermediate/Writing-an-Action-Server-Client/Py.html)
    + [Composing multiple nodes in a single process](https://docs.ros.org/en/foxy/Tutorials/Intermediate/Composition.html)
    + [Launch](https://docs.ros.org/en/foxy/Tutorials/Intermediate/Launch/Launch-Main.html)
-----------------------------------------

## ROS2 architecture
- Example of each architecture of each type of ROS2 node can found [here](https://github.com/ros2/examples/tree/foxy)
- There are 4 types of nodes in ROS2
    + Publisher-Subscriber :: `(Constant stream of publishing and subscribing from each node's data)`
    + Service-Client :: `(Stream of request then response from each node's data)`
    + Action Server-Client :: `(Stream of request then response from each node's data, but with a goal)`

-----------------------------------------

## Tutorials and resources
- [Full ROS2 Documentation](https://docs.ros.org/en/foxy/index.html)