# Localization-using-IMU-sensors-and-python
Vehicle is tracked when GPS disappears outdoors. (maybe while going under a  tunnel or something)(Can be considered for Indoor  localization as well)


The Book1.csv contains the sensor values(magnetometer and distance values obtained from accelerometer) obtained from MPU9250 .
The distance from accelerometer is obtained by double integrating the accelerometer values.
Other alternative is to use the hall sensor and the magnet to calculate the distance.
This can be done by attachiing the hall sensor to the fork of the bike and putting the magnet to the bike spike .

In the localization.ipynb the UTM algorithm is used to track the vehicle and output the lat longs at certain intervals.


Some simple naive algorithm is used to detect the turns using the magnetometer values.
