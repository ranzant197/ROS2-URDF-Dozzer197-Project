# 🤖 ROS2 URDF Dozzer197 Project

This repository contains a complete **ROS2 URDF model** of a hydraulic **Dozzer197 robot**, designed and developed by **Ranjan Tamang**.  
The project demonstrates a fully articulated excavator arm system with multiple **revolute** and **prismatic joints**, **mimic control**, and visualization in **RViz2**.

---

## 🏗️ Project Overview

**Main components:**
- Base frame & station assembly  
- Boom system (dual cylinder + piston with mimic behavior)  
- Dipper & bucket mechanism  
- Dog-bone and H-link structure for motion transfer  
- Full prismatic and revolute joint integration  
- Color-coded mesh visuals for clarity (Red, Blue, Green, White)

---

## 🧠 Key Concepts Implemented

| Feature | Description |
|----------|--------------|
| `Revolute` Joints | Enables rotation between links like boom and dipper |
| `Prismatic` Joints | Simulates hydraulic piston extension and retraction |
| `Mimic` Joints | Couples joint movement (e.g., piston follows boom motion) |
| `RViz2` Visualization | Real-time motion simulation in ROS2 environment |
| `Xacro Macros` | Modular, reusable robot description syntax |

---

## 🛠️ Tools & Technologies

- **ROS2 Humble**  
- **RViz2** for visualization  
- **Fusion 360** for CAD design  
- **Ubuntu 22.04** (dual-boot setup)  
- **Git & VS Code** for version control and editing  

---

## 📂 Folder Structure

my_robot_description/
├── urdf/
│ └── dozzer197.xacro
├── meshes/
│ └── dozzer/
│ ├── Body_frame.stl
│ ├── Station.stl
│ ├── Boom1.stl
│ ├── Boom_cylinder.stl
│ ├── Boom_piston1.stl
│ ├── Dipper.stl
│ ├── Bucket.stl
│ └── ...
├── launch/
│ └── display.launch.py
├── package.xml
└── CMakeLists.txt




---

## 🧩 Launching the Model

```bash
cd ~/ros2_ws/
colcon build --symlink-install
source install/setup.bash
ros2 launch urdf_tutorial display.launch.py model:=/home/ranjan/ros2_ws/src/my_robot_description/urdf/dozzer197.xacro

🌟 Author

👨‍💻 Ranjan Tamang
Robotics Engineer in progress | ROS2 | URDF | Fusion 360 | Python | Japan 🇯🇵
GitHub: ranzant197

























<img width="1920" height="1080" alt="Screenshot from 2025-11-11 20-07-40" src="https://github.com/user-attachments/assets/4257d099-b58a-4e8d-baac-f4304aad8d62" />










