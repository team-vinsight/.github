# Visual-Inertial Navigation for Autonomous UAV Operation in GPS-Restricted Environments

## Team Vinsight

**CS4203 - Research and Development Project**  
Department of Computer Science and Engineering  
University of Moratuwa

---

## � Project Overview

We develop a robust **Visual-Inertial Navigation System (VINS)** for autonomous UAVs in GPS-denied environments. By fusing camera and IMU data, our system ensures precise localization where GPS fails (e.g., indoors, urban canyons) and employs deep learning to filter dynamic objects (like people and vehicles) for enhanced stability.

## 🎯 Key Objectives

*   **GPS-Denied Navigation:** Reliable localization using hybrid Visual-Inertial Odometry (VIO).
*   **Dynamic Robustness:** Masking moving objects to prevent tracking errors in complex scenes.
*   **Embedded Efficiency:** Optimized for real-time performance on NVIDIA Jetson platforms.
*   **Drift Minimization:** Advanced sensor fusion to correct inherent IMU drift.

## 🛠️ Tech Stack

*   **Hardware:** NVIDIA Jetson Orin NX, Stereo Cameras, IMU.
*   **Software:** ROS 2 Humble, PX4 Autopilot, OpenCV, PyTorch.
*   **Algorithms:** ORB-SLAM3 / cuVSLAM, YOLO (Object Detection).

## 📂 Key Repositories

### 🏗️ Core Systems
*   [**drone_ws**](https://github.com/team-vinsight/drone_ws): The main **ROS 2 workspace** containing the complete autonomous flight stack, integrating navigation, control, and customized drivers.

### 🔬 Innovations & Enhancements
*   [**pycuvslam**](https://github.com/team-vinsight/pycuvslam): Fork of **NVIDIA's pycuvslam**, extended with support for custom datasets and new camera sensors.
*   [**pycuvslam-ros2-wrapper**](https://github.com/team-vinsight/pycuvslam-ros2-wrapper): ROS 2 node wrapper for `pycuvslam` to interface with the rest of the drone system.

### 📚 Documentation
*   [**project-proposal**](https://github.com/team-vinsight/project-proposal): LaTeX source code and PDF releases of the official project proposal and research goals.
*   [**knowledge-base**](https://github.com/team-vinsight/knowledge-base): Collection of reference papers, literature reviews, and learning resources.

## 👥 Team Members

*   **D. V. A. I. Delgahagoda** (210113L)
*   **T. T. Kashmeera** (210279A)
*   **K. D. R. P. Rathnayake** (210537N)

**Internal Supervisor:** Prof. Chandana Gamage

