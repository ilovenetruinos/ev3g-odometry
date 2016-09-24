# ev3g-odometry
A set of EV3G Blocks for Mobile Wheeled robots

Using distances and turn angles to navigate a robot is called “odometry”

wheel_circumference = distance / motor_rotations
distance = wheel_circumference * motor_rotations

Pivot turns
One wheel turns while other is stationary
motor_degrees = turn_angle * wheel_track / wheel_radius

Sources of odometry error
Friction
Gear slack 
Wheel slippage 
Battery charge 
Timing issues

References:
http://www.informit.com/articles/article.aspx?p=29383&seqNum=2
http://www.philohome.com/odin/odin.htm
https://docs.google.com/presentation/d/1A24naow7nSux8kLlTG_lh_qklrVWXAcUxS4hRQ4RJGw/present?slide=id.i133
http://www.legoengineering.com/measuring-area-with-a-robot-part-one-follow-the-path/
http://seattlerobotics.org/encoder/200610/Article3/IMU%20Odometry,%20by%20David%20Anderson.htm
https://www.cs.princeton.edu/courses/archive/fall11/cos495/COS495-Lecture5-Odometry.pdf
http://robotics.stackexchange.com/questions/2847/accelerometer-gyro-and-magnetometer-sensor-fusion-in-2d
http://wiki.ros.org/robot_localization
http://www.robotchallenge.org/fileadmin/user_upload/_temp_/RobotChallenge/Tutorial/BeginningNavigation.pdf
https://sourceforge.net/p/lejos/rcx/code/HEAD/tree/trunk/lejos/src/java/classes/josx/robotics/RotationNavigator.java
https://sourceforge.net/p/lejos/nxt/code/HEAD/tree/trunk/classes/src_shared/lejos/robotics/navigation/LegacyNavigator.java
https://sourceforge.net/p/lejos/nxt/code/HEAD/tree/trunk/classes/src_shared/lejos/robotics/navigation/DifferentialPilot.java
