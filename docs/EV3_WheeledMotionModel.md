# Motion Model for a Wheeled robot

The required formulas used to calculate a Pose are:

* wheelCircumference = PI * wheelDiameter
* distance = wheelCircumference * motorRotations
* encoderScaleFactor = (PI * wheelDiameter) / countsPerRevolution
* displacement = (leftEncoderCount + rightEncoderCount) * encoderScaleFactor / 2 
* posX = posX + (displacement * cos(heading)) <- Heading in Radians
* posY = posY + (displacement * sin(heading)) <- Heading in Radians

You can test the calculus in the following Excel to calculate the calculus: [Download Excel](./OdometryCalculusTest.xls)

The odometry error grow with the distance:

![](./docs/images/odometryError1.png)

But it is possible to be increased when the robot turn. Gyro sensor accuracy is able to reduce this kind of error.

![](./docs/images/odometryError2.png)
