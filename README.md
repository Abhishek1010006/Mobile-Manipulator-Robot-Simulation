# Mobile Manipulator Robot Simulation

A ROS 2 Jazzy and Gazebo Sim project that implements a simple mobile manipulator consisting of a differential drive mobile base and a 2-DOF robotic arm. The project demonstrates robot modeling using URDF/Xacro, simulation in Gazebo, and ROS-Gazebo integration.

## Features

- Differential drive mobile robot
- 2-DOF robotic arm
- Camera module
- Modular Xacro-based robot description
- Gazebo Sim integration
- Custom warehouse environment
- RViz visualization support
- ROS-Gazebo topic bridging

## Project Structure

```text
src/
├── my_robot_description/
│   ├── urdf/      # Robot models and Xacro files
│   └── rviz/      # RViz configurations
│
└── my_robot_bringup/
    ├── launch/    # Launch files
    ├── config/    # Gazebo bridge configuration
    └── worlds/    # Custom simulation environments
```

## Robot Architecture

```text
Mobile Manipulator Robot
├── Differential Drive Base
├── 2-DOF Manipulator Arm
├── Camera Sensor
├── Gazebo Simulation
├── RViz Visualization
└── ROS-Gazebo Topic Bridge
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

## Robot Kinematic Tree

```text
base_link
├── left_wheel
├── right_wheel
├── camera_link
└── arm_base
    └── forearm_link
        └── hand_link
```

## Author

**Abhishek Kumar Singh**  
B.Tech CSE, BIT Mesra
