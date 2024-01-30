This is a package for extracting and publishing a sequence of human body skeleton using ZED cameras based on SDK v4.
## Install 
download and move to catkin_ws/src [zed files](https://drive.google.com/file/d/1Jaar8cNrHxhgWvg0E9z-c9KGBaNVyNQe/view?usp=drive_link)
```
git clone https://github.com/mmahdavian/zed_to_pose_sequence.git
cd ../
catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3 --only-pkg-with-deps zed_interfaces

catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3 --only-pkg-with-deps pose_publisher

catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3 --only-pkg-with-deps zed_wrapper

roscore
```
open another terminal and run ```python scripts/body_tracking.py```
