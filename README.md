# Mobile Manipulator Robot Simulation

A ROS 2 Jazzy and Gazebo Sim project that implements a simple mobile manipulator consisting of a differential drive mobile base and a 2-DOF robotic arm. The project demonstrates robot modeling using URDF/Xacro, simulation in Gazebo, and ROS-Gazebo integration.

## Features

- Differential drive mobile robot
- 2-DOF robotic arm
- Modular Xacro-based robot description
- Gazebo Sim integration
- Custom warehouse environment
- RViz visualization support
- ROS-Gazebo topic bridging

## Project Structure

```text
src/
├── my_robot_description/
├── my_robot_bringup/
```

## Dependencies

- Ubuntu 24.04
- ROS 2 Jazzy
- Gazebo Sim

## Build

```bash
cd ~/ros2_ws
colcon build
source install/setup.bash
```

## Running the Simulation

```bash
ros2 launch my_robot_bringup my_robot_gazebo.launch.py
```

```bash
ros2 launch my_robot_description display.launch.py
```

## Robot Kinematic Tree

```text
base_link
└── arm_base
    └── forearm_link
        └── hand_link
```

## Author

**Abhishek Kumar Singh**  
B.Tech CSE, BIT Mesra
