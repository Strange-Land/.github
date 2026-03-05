## Hi there 👋 Welcome to StrangeLand

StrangeLand is a multi-participant simulator for studying human driving behavior and cultural interaction patterns in traffic, helping researchers and developers understand how driving norms vary across contexts and informing the design of future autonomous systems.

**Recommended setup:** Start with the three core packages — [StrangeLandPackage (Core)](https://github.com/Strange-Land/StrangeLandPackage), [StrangeLand Steering](https://github.com/Strange-Land/strangeland.steering), and [StrangeLand Vehicle](https://github.com/Strange-Land/strangeland.vehicle), which together provide the simulator framework, steering hardware integration, and a ready-to-use reference vehicle.

### Repositories

StrangeLand consists of several repositories that together form a comprehensive ecosystem for VR driving simulation and analysis. Below is a brief overview of each repository:

#### 1. [StrangeLandPackage](https://github.com/Strange-Land/StrangeLandPackage)
This Unity package contains the refactored core functionalities of StrangeLand. It is currently being used by several of our collaborators for various projects, and we are actively updating it throughout the collaboration. You can find samples in the package manager to get started.

##### 1.1 Steering
The **[StrangeLand Steering](https://github.com/Strange-Land/strangeland.steering)** package provides a hardware abstraction layer for steering wheels and driving input devices used in StrangeLand simulations. It exposes normalized inputs such as steering, throttle, brake, and common vehicle controls through the `SteeringWheelManager`, allowing vehicle controllers to remain independent of specific hardware SDKs. The package includes example integrations (e.g., Logitech wheels) and samples to test and debug input. Be sure to add the `SteeringWheelManager` to your `GameManagement` scene in Unity. 

##### 1.2 Vehicle
The **[StrangeLand Vehicle](https://github.com/Strange-Land/strangeland.vehicle)** package provides a reference vehicle implementation for StrangeLand. It includes a ready-to-use vehicle prefab with interior interaction elements, mirrors, audio, and a vehicle controller that integrates directly with the `SteeringWheelManager`. Importing the sample allows developers to quickly add a drivable vehicle to a scene and connect it to the StrangeLand interaction and spawning system while remaining fully extensible for custom vehicle setups.

#### 2. [StrangeLand-Base](https://github.com/Strange-Land/StrangeLand-Base/tree/development)
This is the core repository of the StrangeLand system. It contains the foundational code and assets necessary to set up and run the VR driving simulations. Start here if you're new to the StrangeLand ecosystem.

#### 3. [Docs-ReadMe](https://github.com/Strange-Land/Docs-ReadMe)
This repository houses all the documentation related to the StrangeLand project. Here you can find detailed guides, and more to help you navigate and utilize the various components of the StrangeLand system.

*Some Reportistries are still hosted on the originating labs Github*
#### 4. [ReRun](https://github.com/FAR-Lab/Rerun)
It is an addition to StrangeLand that can be used to record the various moving actors in a scene and play them back, facilitating inductive coding for the transpired interactions.
#### 5. [Original Repository](https://github.com/FAR-Lab/CrossCulturalDriving)
The simulator's original repository has a longer history and various issues trackers associated with it that were not migrated to the new StrangeLand-Base repository.

### Future Developments

StrangeLand is continuously evolving. Our future plans for development are divided into two main areas:

#### 1. Studies
We aim to expand the cultural profiling capabilities of StrangeLand by incorporating more diverse driving scenarios, pedestrians, robots, and modern forms of transportation, to studying their effects on driving in different cultural contexts. The goal is to make StrangeLand a universal tool for multiparticipant interactin research moving beyond the traffic and driving context.

#### 2. Technical Improvements
Several enhancements are planned to improve the fidelity and usability of the StrangeLand system. These include better hand-tracking integration, more robust network performance, and the inclusion of additional real-world driving conditions to make the simulations even more realistic. For more details, visit our [Technical Improvements](https://github.com/Strange-Land/Docs-ReadMe/wiki/Technical-Improvments) page.

### History

StrangeLand began as an experimental system developed at Cornell Tech and the Technion in Israel, aiming to understand driving culture through VR. The system has since grown into a versatile tool for driving research, capable of capturing intricate details of driver interaction in various cultural settings. The project has been validated through proof-of-concept studies in multiple locations, showcasing its potential as a powerful tool for driving behavior research.

We invite you to explore, contribute, and help us shape the future of autonomous driving technology by engaging with the StrangeLand project.
