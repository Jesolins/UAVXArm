## UAVXArm ##

The UAVXArm32F4 Board has been available since December 2012 from QuadroUFO and is now at Version 4.

![https://github.com/gke/UAVXArm/blob/master/wiki/graphics/v4.jpg](https://github.com/gke/UAVXArm/blob/master/wiki/graphics/v4.jpg)

### General Specifications ###

UAVXArm32F4 spends most of its time twiddling its thumbs (doing nothing). Control loop and motor updates are at ~500Hz with 2KHz possible.

Standalone mode:

  * STM32F405RG6 with FPU 168MHz (1024Kb Flash/32Kb RAM)
  * 64MBit External Flash (Black Box recorder)
  * MPU6000 Gyro/Accelerometer
  * HMC5983 Magnetometer
  * MS5611 Barometer
  * SPI communications for all sensors
  * Ultrasonic Rangefinder
  * Optional external battery voltage and current monitor
  * Analog and I2C ports for alternative sensors

Receivers:

  * Parallel PPM (8 channels)
  * Compound PPM
  * Spektrum Satellite (1024b and 2048b resolution)
  * Deltang
  * SBus (with external inverter)

A minimum of 4 channels is required for basic flight control with 7 channels being required for RTH and Nav functionality.

Up to 10 drives or servos:

  * FastPWM (490Hz)
  * SyncPWM (400Hz)
  * SyncPWM/8 OneShot 
  * I2C @ 400KHz
  * DCMotors (with optional 6 channel external adapter)

We have used SimonK and BLHeli ESC codes with FastPWM being the sensible minimum for good performance.

All the usual airframe types are supported including conventional fixed wing airframes. 

Attitude Estimation Schemes:

  * Madgwick (IMU)
  * Madgwick (AHRS)

Attitude Control:

  * Angle (default - also called attitude or stable)
  * Rate (commonly called gyro mode)
  * a mix of the above

###Videos and Builds###

There are many many many videos of UAVX on our RCG thread:

http://www.rcgroups.com/forums/showthread.php?t=1093510&page=635#post31446892

Ken the main Alpha tester has a good collection at https://www.youtube.com/user/kb6mccincluding

https://www.youtube.com/watch?v=uYsW6lu7lSA&feature=youtu.be
https://www.youtube.com/watch?v=w_9torIeAb8&feature=youtu.be
https://www.youtube.com/watch?v=faXzluGCzVo&feature=youtu.be





