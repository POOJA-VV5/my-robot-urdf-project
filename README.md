# Mobile Robot URDF Project 🤖

A complete mobile robot URDF model for ROS 2 Jazzy featuring differential drive, camera, and lidar sensors.

## Features
- ✅ Differential drive mobile robot base
- ✅ Two continuous rotating wheels + caster wheel
- ✅ Front-mounted camera sensor
- ✅ Top-mounted 360° lidar sensor
- ✅ Complete physics properties (mass, inertia)
- ✅ Interactive joint control via GUI

## Requirements
- Ubuntu 24.04
- ROS 2 Jazzy
- RViz2
- Joint State Publisher GUI

## Installation
# Clone the repository
cd ~/urdf_ws/src/
git clone git@github.com:POOJA-VV5/my-robot-urdf-project.git my_robot_description

# Build the workspace
cd ~/urdf_ws
colcon build
source install/setup.bash
```

## Usage
```bash
# Launch the robot visualization
ros2 launch my_robot_description display.launch.py
```

This will open:
- **RViz2** with the 3D robot model
- **Joint State Publisher GUI** to control wheel rotation

## Project Structure
```
my_robot_description/
├── urdf/
│   └── my_robot.urdf          # Robot URDF definition
├── launch/
│   └── display.launch.py      # ROS 2 launch file
├── config/
│   └── robot.rviz             # RViz configuration
├── CMakeLists.txt
├── package.xml
└── .gitignore
```

## Robot Specifications

| Component | Dimensions | Material |
|-----------|-----------|----------|
| Base | 0.6m × 0.4m × 0.2m | Blue |
| Wheels | 0.1m radius | Black |
| Caster | 0.05m radius | Grey |
| Camera | 0.05m × 0.15m × 0.05m | Red |
| Lidar | 0.05m radius | Green |

## Future Enhancements
- [ ] Convert to Xacro format for modularity
- [ ] Add Gazebo simulation support
- [ ] Implement functional sensor plugins
- [ ] Add ROS 2 navigation stack integration
- [ ] Add controller configuration

## License
MIT License

## Author
POOJA-VV5
