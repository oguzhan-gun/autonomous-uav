# Autonomous Combat UAV
![ROS2](https://img.shields.io/badge/ROS2-Jazzy-22314E?style=for-the-badge\&logo=ros)

![Gazebo](https://img.shields.io/badge/Gazebo-Simulator-orange?style=for-the-badge)

![PX4](https://img.shields.io/badge/PX4-Autopilot-0055FF?style=for-the-badge)

![MAVLink](https://img.shields.io/badge/MAVLink-Protocol-blue?style=for-the-badge)

![YOLOv11](https://img.shields.io/badge/YOLO-v11-red?style=for-the-badge)

![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=for-the-badge\&logo=opencv)

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge\&logo=cplusplus)

![License](https://img.shields.io/badge/License-Research%20Only-success?style=for-the-badge)


An autonomous air-to-air combat system developed for the **Teknofest Autonomous Combat UAV Competition**. The project focuses on real-time perception, target tracking, predictive guidance, and autonomous interception using ROS 2, Gazebo, PX4, and computer vision.

---

# Demo

<p align="center">

# Demo 
Real-time autonomous target tracking in Gazebo simulation.

<p align="center">
<img src="assets/iha.gif" width="900">
</p>

---

# Overview

This project simulates a two-UAV autonomous combat scenario in which one aircraft detects, tracks, predicts, and intercepts another without human intervention.

The complete autonomy stack includes:

* Real-time object detection
* State estimation
* Multi-sensor fusion
* Predictive target tracking
* Adaptive PID flight control
* MAVLink flight communication
* Autonomous interception logic

The system was successfully developed through the **Critical Design Review (CDR)** phase of the Teknofest Autonomous Combat UAV Competition.

---

# Features

## Real-Time Vision

* YOLOv11-based target detection
* High-frequency perception pipeline
* High-frequency camera input support
* OpenCV-based image processing

---

## State Estimation

* Kalman Filter-based target state estimation
* Velocity estimation
* Angular velocity estimation
* Noise reduction for stable tracking

---

## Predictive Guidance

Instead of following the current target position, the interceptor predicts future target states using an adaptive predictive guidance framework.

Future state estimation considers:

* Target velocity
* Estimated angular velocity
* Current engagement geometry

This approach enables smoother interception while reducing tracking latency during aggressive maneuvers.
---

## Flight Control

Adaptive PID controllers are used for

* Roll
* Pitch
* Yaw
* Throttle

Advanced flight stabilization techniques improve tracking robustness during aggressive maneuvers.

---

## Sensor Fusion

The localization framework combines

* GNSS
* Vision measurements

to improve robustness and positioning accuracy during autonomous engagement.

---

## Autonomous Interception

The project includes a complete interception framework capable of

* Relative positioning
* Lead-angle estimation
* Strategic lower-angle engagement
* Autonomous target locking

---

# Technologies

* ROS 2
* Gazebo
* PX4
* MAVLink
* YOLOv11
* OpenCV
* C++
* Python
* Kalman Filtering
* PID Control
* Sensor Fusion
* Predictive Guidance
* Feed-Forward Control

---

# Results

* Fully autonomous target detection
* Robust predictive tracking
* Real-time interception guidance
* Multi-sensor localization
* PX4 integration
* Successfully completed the Teknofest CDR stage

---

# Future Work

* Multi-target engagement
* Reinforcement Learning-based guidance
* Multi-UAV swarm coordination
* Onboard deployment
* Hardware-in-the-loop testing

---

# License

This repository is intended for research and educational purposes.

# Research

This project is actively maintained and further developed as part of the KARAN UAV Team. Ongoing research focuses on autonomous aerial combat, predictive guidance, sensor fusion, and intelligent UAV systems.

## Support 

If you find this project interesting, consider giving it a ⭐ on GitHub.
