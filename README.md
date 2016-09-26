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
https://sourceforge.net/p/lejos/nxt/code/HEAD/tree/trunk/classes/src_shared/lejos/robotics/navigation/Pose.java
https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/navigation/MovePilot.java
https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/navigation/Move.java
https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/chassis/WheeledChassis.java
https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/navigation/ArcAlgorithms.java
http://www.hmc.edu/lair/E160/labs.html
http://www.hmc.edu/lair/E160/E160-Lecture02-RobotMotion.pdf
http://www.hmc.edu/lair/E160/E160-Lecture03-Odometry.pdf
http://www.hmc.edu/lair/E160/E160-Lecture04-PointTracking.pdf
http://www.hmc.edu/lair/E160/E160-Lecture14-MotionPlanning.pdf
http://www.ohio.edu/people/uijtdeha/12-_-a-comparison-of-line.pdf
https://april.eecs.umich.edu/courses/eecs568_f11/wiki/images/5/5f/Laserscanners.pdf
http://webdiis.unizar.es/~jminguez/MbICP_ICRA.pdf
https://en.wikipedia.org/wiki/Random_sample_consensus
http://www.robosoup.com/2015/11/ransac-line-feature-extraction-from-2d.html
http://www.visual-experiments.com/demo/ransac.js/
http://sarvagyavaish.github.io/RANSAC/
http://cs.gmu.edu/~kosecka/cs682/lect-fitting.pdf
http://stackoverflow.com/questions/11722569/opencv-line-fitting-algorithm
http://blog.daum.net/pg365/87
http://www.ipol.im/pub/art/2012/gjmr-lsd/article.pdf
https://github.com/ab3nd/TinyRobo/blob/2c567728f06eebdb63a06772911e237455a8f4fa/software/catkin_ws/src/sim_robots/src/sim_robots/sim_robots.cpp
