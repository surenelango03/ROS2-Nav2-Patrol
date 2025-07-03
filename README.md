# 🤖 ROS 2 TurtleBot3 Patrol with Nav2 and SLAM

This repository contains my final project from completing the [ROS 2 Navigation Stack (Nav2) with SLAM](https://www.roboticscourse.com/) course by Edouard Renard.

The project simulates a **TurtleBot3 Waffle** robot navigating through a custom mapped house using ROS 2's Navigation Stack. It integrates **SLAM**, **URDF**, **waypoint patrol**, and simulation with **Gazebo**.

---

## 🎯 Key Features

- ✅ ROS 2 Nav2 (Navigation 2) Stack integration
- ✅ SLAM using a custom house environment
- ✅ Python-based patrol control using `nav2_simple_commander`
- ✅ TurtleBot3 robot description with URDF
- ✅ Simulation via Gazebo and RViz
- ✅ Full launch automation

---

## 📁 Repository Structure

```
ros2_nav2_patrol/
├── nav2_test.py                  # Python script for waypoint patrol
├── my_house.yaml                 # SLAM map metadata
├── my_house.pgm                  # SLAM map image file (to be added)
├── urdf/
│   └── turtlebot3_waffle.urdf    # TurtleBot3 URDF description
├── launch/
│   └── turtlebot3_house.launch.py  # Launch file for simulation
└── README.md                     # Project documentation
```

---

## 🛠️ Technologies Used

- ROS 2 Humble
- Python 3
- Gazebo 11
- RViz 2
- `nav2_simple_commander`
- SLAM Toolbox
- URDF, TF, and robot_state_publisher

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ros2_nav2_patrol.git
   cd ros2_nav2_patrol
   ```

2. **Move the project into your ROS 2 workspace and build:**
   ```bash
   cp -r ros2_nav2_patrol ~/ros2_ws/src/
   cd ~/ros2_ws
   colcon build
   source install/setup.bash
   ```

3. **Launch the simulation:**
   ```bash
   ros2 launch your_package_name turtlebot3_house.launch.py
   ```

4. **Run the navigation patrol script:**
   ```bash
   ros2 run your_package_name nav2_test.py
   ```

---

## 🧠 What I Learned

- Implementing Nav2 stack for robot navigation
- Generating and using SLAM maps (`.yaml`, `.pgm`)
- Writing Python navigation scripts with `BasicNavigator`
- Defining robot kinematics and frames in URDF
- Simulating robots in Gazebo and visualizing in RViz
- Launch file configuration using `launch.py`

---

## 📸 Demo



---

## 🎓 Course Reference

- **Course:** [ROS 2 - Navigation Stack with SLAM and Nav2](https://www.udemy.com/course/ros2-nav2-stack)
- **Instructor:** Edouard Renard
---

## 📌 Notes

- Ensure that `my_house.pgm` is added to the repository alongside `my_house.yaml`.
- You must have the TurtleBot3 and Nav2 packages installed and sourced.
- The simulation world used is `turtlebot3_house.world` from `turtlebot3_gazebo`.

---

## 🙌 Acknowledgements

Special thanks to Edouard Renard for the structured guidance throughout the course and to the open-source ROS community.

---
