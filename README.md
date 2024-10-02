SensorTest.java assumes the robot device config uses the LaserRangeSensor option, but only implements one sensor "dist_sensor"
Adding another one should be as easy as making a new LaserRangeSensor object under the first one, and replicating any other lines that refer to "rangeSensor" with the new object instead.
