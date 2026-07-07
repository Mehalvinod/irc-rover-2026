# ROS Interface Contract

Official reference: ROS 2 Humble  
Jazzy users must follow the same topic names, message types, and TF frames.

## Core Topics

| Subsystem | Topic | Type | Frame | Owner |
|---|---|---|---|---|
| LiDAR | /scan | sensor_msgs/msg/LaserScan | laser_link | P14 |
| IMU | /imu/data | sensor_msgs/msg/Imu | imu_link | P12 |
| Odometry | /odom | nav_msgs/msg/Odometry | odom | P12 |
| GPS | /gps/fix | sensor_msgs/msg/NavSatFix | gps_link | P13 |
| Camera Image | /camera/image_raw | sensor_msgs/msg/Image | camera_optical_frame | P15/P19 |
| Camera Info | /camera/camera_info | sensor_msgs/msg/CameraInfo | camera_optical_frame | P15/P19 |
| Mission State | /behavior_tree/mission_state | std_msgs/msg/String | none | P16 |
| Velocity Command | /cmd_vel | geometry_msgs/msg/Twist | base_link | Nav2/P16 |

## Mission States

IDLE  
NAVIGATING  
DETECTING  
RECOVERY  
SUCCESS  
E_STOP  

## Required TF Frames

map  
odom  
base_link  
laser_link  
imu_link  
gps_link  
camera_link  
camera_optical_frame  
