# Self-Driving-Cars
## Autonomous Vehicle Engineering Stack
### Deep Learning, Computer Vision, and Control Systems in the CARLA Simulator

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![CARLA](https://img.shields.io/badge/CARLA-Simulator-green?style=for-the-badge)

## 📌 Overview
This repository contains a comprehensive suite of autonomous driving software developed during the **University of Toronto Self-Driving Cars Specialization**. The projects focus on the "Four Pillars" of autonomy: **Control, Localization, Perception, and Planning.** All systems were validated using the **CARLA high-fidelity simulator**.

## 🚀 Key Projects

### 1. Motion Planning for Self-Driving Cars (The "Final Boss")
Developed a full-stack trajectory planner to navigate a vehicle through a dynamic urban environment with obstacles.
*   **Behavioral Planning:** Implemented a state-machine to handle intersections, stop signs, and lead-vehicle tracking.
*   **Local Planning:** Generated path lattices and velocity profiles using cubic spirals.
*   **Optimization:** Achieved a collision-free path 100% of the time across varying traffic densities.

### 2. State Estimation & Localization
Engineered an **Extended Kalman Filter (EKF)** to fuse data from multiple sensors (GPS, IMU, and Wheel Encoders).
*   **Sensor Fusion:** Successfully mitigated sensor noise to track vehicle position within < 20cm of ground truth.
*   **Error Analysis:** Managed 3D transformation matrices (Rotation/Translation) for precise frame alignment.

### 3. Visual Perception (Computer Vision)
Built a perception pipeline to translate 2D camera data into 3D world coordinates.
*   **Object Detection:** Integrated a CNN-based detector to identify vehicles and pedestrians.
*   **Semantic Segmentation:** Utilized pixel-wise classification to identify "drivable space."
*   **Distance Estimation:** Used pinhole camera geometry and disparity maps to estimate object depth with high accuracy.

### 4. Vehicle Control (Longitudinal & Lateral)
Designed and tuned controllers to ensure smooth path following.
*   **Longitudinal:** Built a **PID Controller** for throttle and brake management.
*   **Lateral:** Implemented a **Pure Pursuit** and **Stanley Controller** to minimize cross-track error at high speeds.
*   **Result:** Maintained a lateral error of less than 0.1m during high-curvature turns.

## 🛠 Tech Stack
*   **Languages:** Python (Primary), C++ (Performance critical modules)
*   **Libraries:** NumPy (Linear Algebra), Matplotlib (Data Viz), OpenCV (Image Processing)
*   **Tools:** CARLA Simulator, Git, Ubuntu/Linux
