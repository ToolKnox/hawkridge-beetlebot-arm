# Beetlebot Arm assembly notes (draft rewrite)

Status: draft rewrite from upstream README. Needs final technical review before marketplace use.

## Mechanical package

The clean upload package currently uses the user-facing STL files from `3D Printing Parts/` and excludes ROS/Gazebo mesh duplicates from `beetlebot_config/meshes/`.

Staged printable parts:

- `Beetlebot - base-1.STL`
- `Beetlebot - base_gear-1.STL`
- `Beetlebot - end_effector_bracket-1.STL`
- `Beetlebot - lowerarm-1.STL`
- `Beetlebot - station_gear-1.STL`
- `Beetlebot - station_lower-1.STL`
- `Beetlebot - station_upper-1.STL`
- `Beetlebot - upperarm-1.STL`
- `ClawPin.STL`
- `GearClaw.STL`
- `Gearclaw2.STL`
- `Gripper Base.STL`
- `Gripper CLaws.STL`
- `brack1.STL`
- `brack2.STL`
- `washer.STL`

## Hardware from upstream README

- Arduino Mega or Uno board; Mega is preferred.
- 2x MG996R continuous/unlocked servos for base and end-effector bracket.
- 2x MG995 servos for arm joints.
- 2x SG90 micro servos for the gripper.
- OV7670 camera module.
- LM2596 buck converter.
- PCA9685 16-channel 12-bit servo driver board.
- 12V DC power source.
- 2x 8x22x7 mm ball bearings.
- Screws, nuts, and jumper wires.

## Known upstream issue to keep visible

The upstream README reports intermittent PCA9685/I2C communication trouble: the Arduino IDE can scan `0x40`, but ROS/i2c tooling can fail to open or talk to the I2C bus. Keep this as a troubleshooting section in the final guide.
