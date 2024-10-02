# Use
Upon building the code, an OpMode will appear, which will run SensorTest.java. You will have to configure the robot's configuration on the driver station- when going to the config and adding a new device on an I2C bus, make sure the "Laser Range Sensor (____)" options show up. If these don't show up, something is wrong with the LaserRangeSensor*.java files. Make sure that line 12 (and any subsequent objects declared like this) has the correct device name passed as an argument. 

# Notes
SensorTest.java assumes the robot device config uses the LaserRangeSensor device, but only implements one sensor "dist_sensor".
Adding another one should be as easy as making a new LaserRangeSensor object under the first one, and replicating any other lines that refer to "rangeSensor" with the new object instead.
One of the sensors (I forgot which one, sorry!) is programmed to respond to the I2C address 0x08, and the other responds to 0x09, hence the need for two nearly identical files. 



# Information
Sensor datasheet: https://www.waveshare.com/wiki/TOF_Laser_Range_Sensor_(B)


