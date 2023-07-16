# ros2-unity-turtlebot3
use turtlebot3 in unity ros2

run unityhub

You need to setup your IP address in unity and then launch this:
```bash
$ ros2 run ros_tcp_endpoint default_server_endpoint --ros-args -p ROS_IP:=127.0.0.1 -p ROS_TCP_PORT:=10000
```

To control turtlebot3
```bash
$ ros2 run teleop_twist_keyboard teleop_twist_keyboard
```


Will appear the movements
```bash
$ ros2 topic echo /cmd_vel
```
