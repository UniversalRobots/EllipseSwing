# EllipseSwing
URCap sample that mainly demonstrates the principle of RobotPositionCallback, WaypointNodeConfig and PoseFactory

Ellipse Swing is a toy example, where a pose is used to define the center point for an ellipse-like movement. The movement is achieved by inserting a pre-configured MoveP program node containing pre-defined and named Waypoint nodes. This example demonstrates how to:

* Obtain a pose for the robot position by requesting the user to define it using the Move Tab
* Name waypoints
* Request the user to move the robot to a given target position

Note:
* The functionality of assigning the Waypoint nodes custom names is only available from URCap API version 1.4.0 (released with PolyScope version 3.7.0/5.1.0)
* Requesting the user to move the robot to a defined center point is only available from URCap API version 1.5.0 (released with PolyScope version 3.8.0/5.2.0).
* From URCap API version 1.6.0 (released with PolyScope version 3.9.0/5.3.0) the use of the deprecated move node config factory (MoveNodeConfigFactory interface) has been replaced with the equivalent builder and the TCP selection of the MoveP node is pre-configured.
* Support for allowing the end user to start from and break on child nodes is only available from URCap API version 1.9.0 (released with PolyScope version 5.6.0).

Information:
* Available from:
  * URCap API version 1.3.0.
  * PolyScope version 3.6.0/5.0.4.

Main API interfaces: UserInteraction, RobotPositionCallback, RobotMovement, RobotMovementCallback, WaypointNodeConfig, MovePMoveNodeConfig, MoveNodeConfigBuilders, MovePConfigBuilder, PoseFactory, Pose, SimpleValueFactory, JointPositions
