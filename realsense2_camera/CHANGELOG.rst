^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package realsense2_camera
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

2.2.20 (2020-11-19)
-------------------
* Add Support - Noetic
* Add demo for using intrinsics from camera_info (show_center_depth.py).
* Add launch option: send logs to ros log file.
* Add feature: get rgb stream from infrared sensor (applies to D415)
* Add feature: Add notification if connected using USB2.1 port.
* Fix bug: Avoid z16h format
* Fix bug: monitor streams frequency without subsribing.
* Fix bug: extrinsincs for right stereo camera refers to the left stereo camera.
* Contributors: Abhijit Majumdar, Isaac I. Y. Saito, Jakub, M-frctrl, Thomas Jespersen, doronhi

2.2.18 (2020-10-26)
-------------------
* Fix bug: Remove parameter with invalid value.
* Fix bug: Colorize the aligned depth image.
* Fix bug: Added pointcloud attributes, when RS2_STREAM_ANY is enabled
* Add feature: enable/disable all sensors. Known issues: parameters persistency and not full power drop.

2.2.17 (2020-09-09)
-------------------
* Fix for ROS on Windows
* Contributors: Lou Amadio, doronhi

2.2.16 (2020-08-06)
-------------------
* Add PID to support D455.
* Improve instability of dynamic reconfigurable options.
* rs_camera.lauch: add "enable_infra" for L515 support.
* Contributors: doronhi

2.2.15 (2020-07-13)
-------------------
* Check runtime version of librealsense2 vs. compiled version and issue a warning is mismatch occurs.
* Support both L515 and L515 pre-prq versions.
* set infra, fisheye, IMU and pose streams to be false by default.
* add d435i-xacro
* comply to ROS Noetic xacro rules (backcompatible with ROS Melodic) 
* Contributors: Marco Camurri, doronhi

2.2.14 (2020-06-18)
-------------------
* Fix compatibility with Librealsense2 Version 2.35.2.
* Fix support for L515.
* Fix urdf issues.
* Add noetic support: change state_publisher into robot_state_publisher
* fix distortion correction model for T265 (equidistant)
* fix stability issues. Stop sensors at program termination.
* Contributors: Brice, Helen Oleynikova, doronhi

* upgrade version to 2.2.13
* fix ctrl-C closing issues.
* handle device creation exceptions.
* support LiDAR camera L515.
* optimize pointcloud. Contributors: Davide Faconti
* fix usb port id parsing issues.
* Add eigen dependency - missing for Melodic. Contributors: Antoine Hoarau
