# shadow_description

ROS 2 package with the Shadow robot model: URDF, meshes, and RViz configuration.

## Contents
- `urdf/shadow.urdf`: URDF model (exported from SolidWorks).
- `meshes/`: associated STL meshes.
- `rviz2/default.rviz`: RViz configuration.
- `launch/display.launch.py`: launches `robot_state_publisher`, `joint_state_publisher_gui`, and RViz.

## Requirements
- ROS 2
- `robot_state_publisher`
- `joint_state_publisher_gui`
- `rviz2`

## Usage
```bash
colcon build --packages-select shadow_description
source install/setup.bash
ros2 launch shadow_description display.launch.py
```

## License
Apache-2.0. See `LICENSE`.
