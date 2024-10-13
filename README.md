# ros2_workshop_nsu_2024
Material for the ROS 2 workshop hosted by IEEE NSU RAS SBC on Oct 6 & 7, 2024

---------

## Going over the basics with Turtlesim

Run TurtleSim
```
ros2 run turtlesim turtlesim_node
```

Run Turtle Teleop
```
ros2 run turtlesim turtle_teleop_key
```

List Nodes
```
ros2 node list
```

Spawn Another Turtle
```
ros2 service call /spawn turtlesim/srv/Spawn '{"x": 5.0, "y": 3.0, "theta": 2.0, "name": "clark"}'
```

Remap Turtle Teleop
```
ros2 run turtlesim turtle_teleop_key --ros-args --remap __node:=clark_controller --remap turtle1/cmd_vel:=clark/cmd_vel
```