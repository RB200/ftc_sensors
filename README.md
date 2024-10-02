# Notes
SensorTest.java assumes the robot device config uses the LaserRangeSensor device, but only implements one sensor "dist_sensor".
Adding another one should be as easy as making a new LaserRangeSensor object under the first one, and replicating any other lines that refer to "rangeSensor" with the new object instead.
One of the sensors (I forgot which one, sorry!) is programmed to respond to the I2C address 0x08, and the other responds to 0x09, hence the need for two nearly identical files. 

# Information
Sensor datasheet: https://www.waveshare.com/wiki/TOF_Laser_Range_Sensor_(B)
