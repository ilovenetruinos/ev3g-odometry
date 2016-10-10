# ev3g-odometry

A EV3G project to develop to implement the Motion model using Tacho Motors and EV3 Gyros.

## Documentation

* Motion Model for a Wheeled robot
* Motion Model for a Robot using a Gyro Sensor
* [Remote Debugging with Bluetooth](./docs/EV3_Bluetooth.md)
* Trigonometry

# Maths

* wheelCircumference = PI * wheelDiameter
* distance = wheelCircumference * motorRotations
* displacement = (leftEncoderCount + rightEncoderCount) * encoderScaleFactor / 2 
* encoderScaleFactor = PI * wheelDiameter / countsPerRevolution
* posX = posX + displacement * cos(heading)
* posY = posY + displacement * sin(heading)

**Sources of odometry error:**

* Friction
* Gear slack 
* Wheel slippage 
* Battery charge 
* Timing issues

## References:

* [EV3Dev Mapping](http://www.ev3dev.org/projects/2016/08/07/Mapping/) (Thanks Bmegli)
* [Odin](http://www.philohome.com/odin/odin.htm)
* [Cartographer](https://github.com/googlecartographer/cartographer)
* http://seattlerobotics.org/encoder/200610/Article3/IMU%20Odometry,%20by%20David%20Anderson.htm
* https://www.cs.princeton.edu/courses/archive/fall11/cos495/COS495-Lecture5-Odometry.pdf
* https://sourceforge.net/p/lejos/rcx/code/HEAD/tree/trunk/lejos/src/java/classes/josx/robotics/RotationNavigator.java
* https://sourceforge.net/p/lejos/nxt/code/HEAD/tree/trunk/classes/src_shared/lejos/robotics/navigation/LegacyNavigator.java
* https://sourceforge.net/p/lejos/nxt/code/HEAD/tree/trunk/classes/src_shared/lejos/robotics/navigation/DifferentialPilot.java
* https://sourceforge.net/p/lejos/nxt/code/HEAD/tree/trunk/classes/src_shared/lejos/robotics/navigation/Pose.java
* https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/navigation/MovePilot.java
* https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/navigation/Move.java
* https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/chassis/WheeledChassis.java
* https://sourceforge.net/p/lejos/ev3/code/ci/master/tree/ev3classes/src/lejos/robotics/navigation/ArcAlgorithms.java


