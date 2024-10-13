# ros2_workshop_nsu_2024
Material for the ROS 2 workshop hosted by IEEE NSU RAS SBC on Oct 6 & 7, 2024

---------

## Creating a custom ROS2 package

Create a folder in your home directory
```
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws/src
```

Create a ROS2 package
```
ros2 pkg create --build-type ament_python --node-name my_node my_package
```

Build the project
```
cd ~/ros2_ws
colcon build --symlink-install
```

Source the workspace (we'll be adding it to our .bashrc to make sure all terminals have access to this workspace)
```
echo "source ~/ros2_ws/install/setup.bash" >> ~/.bashrc
```

