# Realsense D435i Description
This package contains the URDF description and gazebo plugins for the Intel Realsense D435i camera.

## Dependencies
This package depends on the following packages:
- [realsense_gazebo_plugin](https://github.com/pal-robotics/realsense_gazebo_plugin)

## Usage
To add the camera to your robot, add the following to your URDF file:
```xml
<xacro:include filename="$(find realsense_d435i_description)/urdf/_d435i.urdf.xacro" />
<xacro:realsense_d435i parent="base_link" name="camera" unite_imu_method="linear_interpolation">
	<origin xyz="0.064 0 0.09" rpy="0 0 0"/>
</xacro:realsense_d435i>
```

## Credits
This package is a cleaned up version of the [Turtlebot3_with_Realsense_D435i](https://github.com/SuaPiamsuk/Turtlebot3_with_Realsense_D435i) package by [SuaPiamsuk](https://github.com/SuaPiamsuk).