# 🎮 Virtual Reality Rehabilitation Game for Cerebral Palsy Patients  

### 🧠 Unity | 🕹️ Google VR SDK | 📡 BNO055 Sensor Integration | 🤖 Machine Learning  

---

## 🩵 **Overview**

This project presents an **interactive Virtual Reality (VR) rehabilitation game** designed to assist **Cerebral Palsy (CP)** patients with **motor skill therapy** in an immersive, motivating, and adaptive environment.  
Developed using **Unity** and integrated with **Google’s VR SDK**, the system connects **real-world physical movements** to **virtual gameplay** through sensor-based motion tracking.  

Machine Learning (specifically **Linear Regression**) is applied to accurately **map and predict real-world sensor coordinates** to **virtual environment positions**, ensuring smooth and natural in-game motion.

---

## 🏗️ **Core Components**

### 🧩 1. Unity Game Engine  
- Built the 3D VR environment using **Unity** for real-time rendering and physics.  
- Designed interactive elements and customizable therapy exercises for engaging gameplay.  
- Integrated **Google VR SDK** for immersive head-tracking and camera control.

### 📡 2. BNO055 Sensor Integration  
- Used **BNO055 IMU sensors** (gyroscope + accelerometer + magnetometer) to capture limb motion.  
- Developed a data pipeline to stream sensor coordinates to the Unity environment.  
- Linked physical limb movements directly to the player avatar for accurate mirroring in VR.

### 🤖 3. Machine Learning Model  
- Collected synchronized **real-world sensor data** and **VR coordinate data**.  
- Trained a **Linear Regression model** to establish the mapping function between the two coordinate systems.  
- Enabled dynamic calibration — adapting to different users and movement ranges.

### 🎥 4. Demonstration  
- The repository includes an [🎥 **MP4 video demo**](./VR_Game_Video.mp4) showcasing the full system in action — from real-world movement capture to VR interaction. 

---

## 🌍 **System Architecture**

```plaintext
[ BNO055 Sensor Data ] → [ Data Processing + ML Model ] → [ Unity Environment via Google VR SDK ] → [ Real-time Visual Feedback ]
