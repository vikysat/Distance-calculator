# Distance-calculator

This ROS2 node subscribes to /turtle1/pose, extracts the turtle’s (x, y) position, computes the Euclidean distance from the origin (0, 0), and publishes the result to a new topic: /turtle1/distance_from_origin.

Features:
 
Subscribes to /turtle1/pose (type: turtlesim/msg/Pose)
Computes: distance = sqrt(x² + y²)
Publishes distance to /turtle1/distance_from_origin (type: std_msgs/msg/Float64)

Requirements:

ROS2 (e.g. Humble, Foxy, or Rolling)
turtlesim package
