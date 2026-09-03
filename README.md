# TurtleBot3 ROS 2 Python Study Workspace

This repository is a personal study workspace for learning how to use **ROS 2** with TurtleBot3. It follows step-by-step tutorials and practical examples involving Python nodes, ROS 2 topics, services, messages, simulation, teleoperation, navigation, and Dynamixel motor control.

The workspace includes source packages under `src/`, together with generated `build/`, `install/`, and `log/` directories created by the ROS 2 build process. These generated directories are local build artifacts and must not be published as source code.

## What This Workspace Contains

The source tree is based on official open-source projects, including:

- TurtleBot3 ROS 2 packages for bringup, descriptions, examples, teleoperation, navigation, and simulation.
- TurtleBot3 message, service, and action definitions.
- Dynamixel SDK packages and custom interfaces used for motor communication.
- Python-based ROS 2 examples and nodes used for study and experimentation.

This workspace is intended for educational practice. The code was assembled by following tutorials and setup instructions to learn ROS 2. It is not presented as an original implementation or as a replacement for the official documentation.

## Building the Workspace

From the workspace root, source the ROS 2 installation and build the packages with `colcon`:

```bash
source /opt/ros/<ros2-distribution>/setup.bash
colcon build --symlink-install
source install/setup.bash
```

Replace `<ros2-distribution>` with the ROS 2 distribution installed on your system, such as `humble` or `jazzy`.

## Version-Control Policy

Only the source tree in `src/` should be committed to the training repository. The root `.gitignore` excludes the generated `build/`, `devel/`, and `install/` directories, as well as `log/` and Python cache files. Do not commit compiled packages, generated setup files, logs, or other local build output.

The GitHub repository for this study workspace is:

https://github.com/RodsSarno/turtlebot3_training

## Running Examples

After building and sourcing the workspace, use the official package documentation to select the appropriate launch files and commands. Typical ROS 2 commands include:

```bash
ros2 pkg list | grep turtlebot3
ros2 topic list
ros2 node list
```

Simulation, navigation, hardware, and camera-related examples may require additional ROS 2 dependencies, Gazebo configuration, robot hardware, or sensor drivers.

## Attribution, License, and Ownership

The TurtleBot3 ecosystem is maintained by **ROBOTIS** under the open-source **Apache License 2.0**. This workspace uses ROBOTIS's official TurtleBot3 packages as the foundation for personal study, learning, and possible modifications.

The original TurtleBot3, TurtleBot3 simulation, TurtleBot3 messages, and Dynamixel SDK materials belong to their respective authors and maintainers. I do not claim ownership of those materials. Please consult the original repositories and license files in the source tree for the authoritative copyright, attribution, and redistribution terms.

Official resources:

- [TurtleBot3 by ROBOTIS](https://github.com/ROBOTIS-GIT/turtlebot3)
- [TurtleBot3 simulations](https://github.com/ROBOTIS-GIT/turtlebot3_simulations)
- [TurtleBot3 messages](https://github.com/ROBOTIS-GIT/turtlebot3_msgs)
- [DynamixelSDK by ROBOTIS](https://github.com/ROBOTIS-GIT/DynamixelSDK)
- [TurtleBot3 e-Manual](https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/)

## AI Disclosure

This README was created with the assistance of artificial intelligence (AI).
