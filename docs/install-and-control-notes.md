# Beetlebot Arm install/control notes (draft rewrite)

Status: draft rewrite from upstream README. Needs testing before publication.

## Simulation path

Upstream targets Ubuntu 18.04 with ROS Melodic, RViz, MoveIt, Gazebo, rosserial, and OpenCV.

Primary upstream commands:

```bash
mkdir -p ~/beetlebot_setup/src
cd ~/beetlebot_setup/src
git clone https://github.com/Kartik-Singhal26/Beetlebot-Arm
catkin_make
cd ~/beetlebot_setup
source devel/setup.bash
roslaunch beetlebot_moveit_config demo.launch
roslaunch beetlebot_moveit_config gazebo.launch
```

## Real arm teleoperation path

Upstream uses PCA9685 over I2C and ROS i2cpwm board support:

```bash
sudo apt-get install libi2c-dev
mkdir -p catkin_ws/src
cd ~/catkin_ws/src
git clone https://gitlab.com/bradanlane/ros-i2cpwmboard.git
cd ..
catkin_make
source devel/setup.bash
roscore
rosrun i2cpwm_board i2cpwm_board
```

## Modernization notes

- Rewrite Ubuntu 18.04/ROS Melodic instructions for a current supported ROS path or clearly label them as legacy.
- Verify PCA9685 wiring/power and document separate servo power from logic power.
- Add a concise non-ROS Arduino/PCA9685 smoke test if possible before publishing.
