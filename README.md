# VIP-UV-Robot
UV Bot Autonomous Setup

# Overview

This code implements an autonomous setup for a UV Bot using ROS (Robot Operating System) and Python. The UV Bot follows a wall using data from a laser scanner and adjusts its trajectory to maintain a desired distance from the wall.

# Prerequisites

ROS installed on your system.
Python environment with NumPy and Matplotlib installed.
# Setup

1. Clone this repository to your local machine:
git clone <repository-url>

2. Navigate to the project directory:
cd uv-bot-autonomous-setup

3. Install dependencies:
pip install numpy matplotlib rospy

# Usage

1. Launch ROS:
roscore

2. Run the UV Bot autonomous setup:
python autonomous_setup.py

# ROS Topics

Subscribed Topics:
/scan: Laser scan data from the UV Bot.

Published Topics:
/cmd_vel: Drive commands for controlling the UV Bot's movement.

# Parameters

SIDE: Set to -1 for the right side or 1 for the left side.
VELOCITY: Desired velocity of the UV Bot.
DESIRED_DISTANCE: Target distance from the wall.
# Details

The UV Bot follows a wall by analyzing laser scan data to detect the proximity of the wall.
A proportional controller is used to adjust the UV Bot's steering angle based on the error in the angle and distance to the wall.

# License

This project is licensed under the MIT License - see the LICENSE file for details.

# Acknowledgments

Thanks to the ROS community for providing a robust robotics middleware.
