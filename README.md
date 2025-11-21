# ros1-

将在一张中的双目图像分割为左右两张图片发布出去。

默认输入的 ros 话题为 `/usb_cam/image_raw`，发布的左右两张图像的话题为 `/left_cam/image_raw`、`/right_cam/image_raw`，可通过 launch 修改话题。

使用方法：

```bash
mkdir ros_ws && cd ros_ws
mkdir src && cd src
git clone https://github.com/heurry/ros1-.git
cd ..
catkin_make
roslaunch camera_split camera_split.launch
```
