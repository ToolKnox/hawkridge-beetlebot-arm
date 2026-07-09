# Beetlebot Arm

Apache-2.0 3D printed 5-DOF robotic arm with ROS simulation, printable CAD files, Arduino/PCA9685 servo electronics, and clear BOM evidence.

## Installation / quick start

## Project

Beetlebot Arm

Apache-2.0 3D printed 5-DOF robotic arm with ROS simulation, printable CAD files, Arduino/PCA9685 servo electronics, and clear BOM evidence.

## Quick start

1. Download the printable files from Printables: https://www.printables.com/model/1776625-beetlebot-arm
2. Download this GitHub repository as a ZIP, or clone it:

   ```bash
   git clone https://github.com/ToolKnox/hawkridge-beetlebot-arm.git
   ```

3. Use `source/upstream/` for the mirrored software, firmware, PCB, CAD-source, and upstream documentation.
4. Use the Bill of Material PDF attached to the Printables Documentation section for parts planning.
5. Read the project-specific notes below before powering electronics or uploading firmware.

## Software / firmware setup

- For the ROS path, use a catkin workspace and source the workspace before launching MoveIt/Gazebo/teleoperation nodes. The upstream README remains in `source/upstream/README.md`.
- PCB/Gerber/electronics design files are mirrored under `source/upstream/`; open them with the original toolchain noted by the file type, such as KiCad, Altium, or CAM/Gerber viewers.

## Main software/config files

- `source/upstream/beetlebot_config/config/joint_names_beetlebot_config.yaml`
- `source/upstream/beetlebot_config/launch/display.launch`
- `source/upstream/beetlebot_config/launch/gazebo.launch`
- `source/upstream/beetlebot_config/package.xml`
- `source/upstream/beetlebot_config/urdf/beetlebot_config.urdf`
- `source/upstream/beetlebot_moveit_config/config/chomp_planning.yaml`
- `source/upstream/beetlebot_moveit_config/config/fake_controllers.yaml`
- `source/upstream/beetlebot_moveit_config/config/joint_limits.yaml`
- `source/upstream/beetlebot_moveit_config/config/kinematics.yaml`
- `source/upstream/beetlebot_moveit_config/config/ompl_planning.yaml`
- `source/upstream/beetlebot_moveit_config/config/ros_controllers.yaml`
- `source/upstream/beetlebot_moveit_config/config/sensors_3d.yaml`
- `source/upstream/beetlebot_moveit_config/launch/beetlebot_config_moveit_controller_manager.launch.xml`
- `source/upstream/beetlebot_moveit_config/launch/beetlebot_config_moveit_sensor_manager.launch.xml`
- `source/upstream/beetlebot_moveit_config/launch/chomp_planning_pipeline.launch.xml`
- `source/upstream/beetlebot_moveit_config/launch/default_warehouse_db.launch`
- `source/upstream/beetlebot_moveit_config/launch/demo.launch`
- `source/upstream/beetlebot_moveit_config/launch/demo_gazebo.launch`
- `source/upstream/beetlebot_moveit_config/launch/fake_moveit_controller_manager.launch.xml`
- `source/upstream/beetlebot_moveit_config/launch/gazebo.launch`
- … 15 more software/config files under `source/upstream/`.

## PCB / electronics design files

- `source/upstream/beetlebot_config/urdf/beetlebot_config.csv`

## Upstream documentation mirrored here

- `source/upstream/README.md`

## Original source

https://github.com/Kartik-Singhal26/Beetlebot-Arm


## Where to find things

- Printables model and printable files: https://www.printables.com/model/1776625-beetlebot-arm
- Bill of Material: `Beetlebot Arm Bill of Material.pdf` in the Printables Documentation section
- Full mirrored upstream source/software/PCB files: `source/upstream/`
- Source asset index: `docs/source-assets.md`
- Standalone install/build guide: `docs/INSTALLATION.md`

