# Visual-Inertial Navigation for Autonomous UAV Operation in GPS-Restricted Environments

## Team Vinsight

**CS4203 - Research and Development Project**  
Department of Computer Science and Engineering  
University of Moratuwa

---

## 📖 Project Overview

Unmanned Aerial Vehicles (UAVs) are rapidly transforming industries like agriculture, logistics, and surveillance. However, their reliable operation often depends on GPS, which is prone to failure in "GPS-restricted" environments such as urban canyons, indoor facilities, and dense forests.

This project proposes a robust **Visual-Inertial Navigation System (VINS)** specifically engineered for autonomous UAV operation in these challenging scenarios. By integrating visual data from onboard cameras with inertial measurements from IMUs, our system enables precise localization and navigation without relying on external satellite signals.

## ⚠️ Problem Statement

Standard GPS-based navigation fails in environments with signal obstruction, multipath propagation, or interference. While visual and inertial systems offer an alternative, they face significant challenges:
*   **IMU Drift:** Inertial sensors accumulate error over time, leading to unbounded trajectory drift.
*   **Dynamic Environments:** Moving objects and low-texture scenes confuse traditional visual tracking algorithms.
*   **Computational Constraints:** Running sophisticated SLAM (Simultaneous Localization and Mapping) algorithms on onboard UAV hardware is resource-intensive.

## 💡 Proposed Solution

We are developing a hybrid, optimization-based VINS that combines:
1.  **Geometric SLAM:** Leveraging **ORB-SLAM3** for utilizing its state-of-the-art accuracy and efficiency in static environments.
2.  **Deep Learning:** Augmenting the geometric backbone with a lightweight object detection model (e.g., YOLO variants) to identify and mask dynamic objects (people, vehicles) that would otherwise corrupt the mapping process.

This approach ensures "best of both worlds" performance: the precision of geometric methods and the semantic understanding of modern AI, all optimized to run in real-time on embedded hardware.

## 🎯 Research Objectives

1.  **Minimize IMU Drift:** Effective fusion of visual and inertial data to maintain stable localization.
2.  **Robust Visual Tracking:** Enhance performance in low-texture and dynamic environments.
3.  **Real-Time Performance:** Optimize algorithms to run efficiently on resource-constrained platforms (e.g., NVIDIA Jetson).
4.  **Environmental Resilience:** Improve system stability under poor lighting and motion blur conditions.

## 🛠️ Technology Stack

*   **Hardware:** NVIDIA Jetson Orin NX (8GB), Stereo/Mono Cameras, IMU.
*   **Flight Stack:** PX4 Autopilot, MAVLink, MAVSDK/MAVROS.
*   **Software framework:** ROS 2 (Humble), OpenCV, Eigen, Ceres/G2O.
*   **Core Algorithms:** ORB-SLAM3 (VIO mode), YOLO-Tiny/Nano for object detection.

## 👥 Team Members

*   **D. V. A. I. Delgahagoda** (210113L)
*   **T. T. Kashmeera** (210279A)
*   **K. D. R. P. Rathnayake** (210537N)

**Internal Supervisor:** Prof. Chandana Gamage

