Understanding VL6180X Time of Flight Sensor:

The VL6180X is a ToF sensor that measures the distance to an object by emitting a pulsed infrared laser and measuring the time it takes for the light to bounce back. The sensor can measure distances with high accuracy, making it suitable for applications like gesture recognition, proximity sensing, and range finding.

Learning Process:

I began by studying the datasheet and documentation provided by the sensor manufacturer to understand its specifications, pin configuration, and communication protocol. Setting up the hardware involved connecting the sensor to a microcontroller (in our case, a Particle Photon 2) and supplying the necessary voltage and ground connections. We wrote code to communicate with the sensor via the I2C interface, which allowed us to initiate measurements and read distance data. Calibration was a crucial step to ensure accurate distance measurements, and we learned how to adjust sensor settings for different applications. Experiences:

The VL6180X sensor performed exceptionally well in tests, the only road block was that since it used  I2C communication and the addresses of all the TOF sensors where the same (0x31 in this case), Particle could not differentiate input from the sensors. 

I tried resolving this by using the shutdown (SHDN) pin in the breakout board to individually shutdown the sensors with a 10ms delay, and read from only a single sensor at a time. This turned out to be a not so smooth operation as it was not giving consistent output as an individual sensor. The other option would have been to use an I2C multiplexer, but delivery dates for it were post the project due date.

In the same time, I started facing issues with my particle board- it was not flashing for almost an entire day, even though I resorted to reset it. Luckily it started working again after a 3rd reset.  As the  deadline was getting closer, I had to look for alternate for the TOF sensor. I considered using an IR sensor, with a reduced accuracy(wider sensing cone)



Sharp 2Y0A710 IR Sensor: The Sharp 2Y0A710 is an analog infrared (IR) proximity sensor that calculates the distance to an object based on the intensity of reflected infrared light. These sensors are commonly used in robotics and obstacle avoidance applications.

I started by examining the sensor's datasheet and pinout to understand how to connect it to photon. Writing code to interpret the analog sensor data and calibrating the sensor was an essential part of the learning process.

The Sharp 2Y0A710 IR sensor is straightforward to use, making it suitable for basic distance-sensing applications, though the sensing cone is wider for making a wind chime. I found the analog nature of the sensor to be both a strength and a limitation; it provided raw data for custom calibration but at the cost of lost accuracy compared to TOF sensors. 

I taped 4 sensors on the table to empirically determine the distances between the sensors and the distance to the striker. With this measurements, created a 3D model for the final chimes and got it laser cut on acrylic. 




