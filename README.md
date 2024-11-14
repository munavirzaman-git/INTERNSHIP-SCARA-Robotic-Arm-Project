Docking System for 3-DOF Planar Robotic Manipulator
This project focuses on developing a docking system using a 3-degree-of-freedom (3-DOF) planar robotic manipulator. The objective is to design and control a robotic arm capable of precise positioning and alignment with target objects. The project involves simulation, motion planning, hardware integration, and performance evaluation to create a functional docking system with potential applications in space, manufacturing, and logistics.

Project Overview
The project encompasses the following stages:

Simulation and Modeling: Using ROS, RViz, and Gazebo for realistic environment creation, allowing visualization and testing of the RRR robot model.
Robot Description: Creation of a URDF model to define the robot arm's structure, dimensions, and joint properties.
Motion Planning and Control: Integration of MoveIt for trajectory planning and inverse kinematics.
Hardware Interfacing: Implementation of object position detection, workspace identification, and calibration with Dynamixel motors.
Performance Evaluation: Validating physical movements against simulation results and ensuring consistency.
Table of Contents
Objectives
Installation & Setup
Robot Modeling and Simulation
Motion Planning with MoveIt
Hardware Setup and Calibration
Results
Future Work
Objectives
Design a 3-DOF robotic manipulator capable of precise docking.
Develop simulation, motion planning, and inverse kinematics.
Implement hardware for real-world validation and compare with simulations.
Installation & Setup
Requirements
Ubuntu 20.04: OS for ROS Noetic compatibility.
ROS Noetic: Robotic Operating System for integration and control.
Gazebo: For realistic simulation and visualization.
RViz: For visualizing robot states and navigation paths.
Installation
Install ROS Noetic: ROS Noetic Installation Guide
Install Gazebo: Included with ROS Noetic.
Clone this Repository:
bash
Copy code
git clone https://github.com/yourusername/docking-system.git
cd docking-system
Install Dependencies:
bash
Copy code
sudo apt-get update
rosdep install --from-paths src --ignore-src -r -y
Robot Modeling and Simulation
Define Robot URDF Model:

The URDF model specifies the robot's structure, dimensions, and joint properties. This is essential for simulation and visualization in Gazebo and RViz.
Develop CAD Model:

Use SolidWorks to create a 3-wheel mobile base and export it to the ROS environment for realistic simulation.
Create Simulation Environment:

Set up Gazebo and RViz to visualize and simulate the robot’s movement and docking process.
Load URDF into RViz for joint and path visualization.
Motion Planning with MoveIt
Set Up MoveIt Package:

Create a MoveIt package to handle the motion planning, inverse kinematics, and trajectory control of the robotic manipulator.
Configure Motion Planning:

Use MoveIt’s planning tools to develop and test trajectory algorithms and to create smooth, efficient paths for the robot arm.
Run Motion Tests:

Simulate the motion plans in Gazebo and visualize in RViz to ensure path accuracy.
Hardware Setup and Calibration
Setup Hardware Components:

Interface and test Dynamixel motors and other electronic components for smooth physical movement.
Camera Calibration:

Calibrate cameras for workspace and object position detection.
Workspace Point Identification:

Identify specific points within the workspace for docking, based on sensor inputs and camera feedback.
Test Hardware Movements:

Validate the real-world movements of the robot arm, comparing them with simulation results for consistency.
Results
Simulation Performance: The system was successfully simulated using Gazebo and RViz, demonstrating accurate motion planning and alignment.
Hardware Validation: Physical robot arm movements were consistent with simulations, proving the efficacy of the docking system.
Future Work
Performance Enhancements: Explore advanced control strategies and sensing technologies.
Advanced Sensing Integration: Improve object detection accuracy with advanced sensors.
Application Optimization: Optimize for specific docking scenarios in logistics or manufacturing.
