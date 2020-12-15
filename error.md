#### Running command: "make cmake_check_build_system"
#### Running command: "make -j4 -l4"

pip install -U rosdep rosinstall_generator wstool rosinstall six vcstools


Python 3 users in ROS Melodic and earlier: note, if you are building ROS from source to achieve Python 3 compatibility, and have setup your system appropriately (ie: have the Python 3 versions of all the required ROS Python packages installed, such as catkin) the first catkin_make command in a clean catkin workspace must be:

$ catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3
This will configure catkin_make with Python 3. You may then proceed to use just catkin_make for subsequent builds.



sudo apt-get install cmake python-catkin-pkg python-empy python-nose python-setuptools libgtest-dev build-essential
