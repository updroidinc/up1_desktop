# up1_desktop #

Desktop ROS packages for the UpDroid UP1, which may pull in graphical dependencies. The contents of this metapackage is software that must be run on a desktop PC, with or without a connected simulated/physical robot.

# Packages #

 - up1_viz : Visualization (rviz and image_view).

# Usage #

To view the UP1 urdf model in rviz with manual joint control:
```bash
roslaunch up1_viz view_model.launch gui:=true
```

With cameras connected to your desktop machine and nodes publishing the image data to the appropriate (i.e. usb_cam_node), visualize with stereo image processing (which is off by default):
```bash
roslaunch up1_viz image_view.launch stereo:=true
```
