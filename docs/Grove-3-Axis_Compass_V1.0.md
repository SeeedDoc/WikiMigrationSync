<!-- 
+++
title       = "Grove - 3-Axis Compass V1.0"
+++
 -->

# Grove - 3-Axis Compass V1.0

Introduction
------------

![](assets/Grove-3-Axis_Compass_V1.0/img/Grove-3-Axis_Compass_V1.0.jpg)

This 3-axis digital compass features a low field magnetic sensing multi-chip module HMC5883L, which provides up to 1° to 2° heading accuracy. HMC5883L consists of high-resolution HMC118X series magneto-resistive sensors, as well as Honeywell developed ASIC containing amplification, automatic degaussing strap drivers, offset cancellation and 12 bit ADC. With peripheral power management circuit added, this is an easy to use and reliable compass module for low cost compassing and magnetometry.

[![](assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-3-Axis-Digital-Compass-p-759.html)

Specifications
--------------

-   Input Voltage: 3.3V, 5V
-   Sleep Mode Current: 2.5uA
-   Measurement Mode Current: 640uA
-   High resolution
-   Easy to control I2C interface
-   Compatible with either 3.3V or 5.0V development platform
-   Max 116Hz output rate
-   High heading accuracy

Demonstration
-------------

### With [Arduino](/index.php?title=ArduinoAndaction=editAndredlink=1 "Arduino")

This demo is going to show you how to read raw data, how to calibrate the data with your local magnetic declination angle and how to get heading angle.

First off, before any action you are going to take, you need to prepare a parameter you are going to use in your demo. That's your local magnetic declination.

You can find it out in degree via [the magnetic declination webpage](http://www.magnetic-declination.com/). For example, mine is -2°37’, which is -2.617 degree.

Then transfer it from degree to radians, and there you get the "declinationAngle". For example, in my case, declinationAngle = -2.617 \* π / 180 = -0.0456752665 rad. Three significant figures are enough. So I would shorten it into -0.0456 rad. And this is the parameter you are going to replace the value of "declinationAngle" in the demo code with.

Now let's start to run your compass.

1. Plug the 3-axis compass into the I2C port of Grove - Base Shield.

2. Download the library file: [Digital Compass Library](assets/Grove-3-Axis_Compass_V1.0/res/Digital_Compass.zip). Unzip it into the libraries file of Arduino IDE by the path: ..\\arduino-1.0.1\\libraries.

3. Open the demo by the path:File ->Example ->Digital Compass ->HMC5883L_Example.

    ![](assets/Grove-3-Axis_Compass_V1.0/img/Digital_Compass1.jpg)

4. Replace the value of variable "declinitionAngle" with the one you've figured out already.

5. Upload the Code. Please click [here](/Upload_Code) if you do not know how to upload.

6. Check the output result by opening the serial monitor.

    ![](assets/Grove-3-Axis_Compass_V1.0/img/Digital_Compass2.jpg)

### With [Raspberry Pi](/GrovePiPlus "GrovePi+")

1.You should have got a raspberry pi and a grovepi or grovepi+.

2.You should have completed configuring the development enviroment, otherwise follow [here](/GrovePiPlus#Introducing_the_GrovePi.2B).

3.Connection

-   Plug the sensor to grovepi socket i2c-x(1~3) by using a grove cable.

4.Navigate to the demos' directory:

       cd yourpath/GrovePi/Software/Python/

-   To see the code

```
    nano grove_compass_lib.py       
    nano grove_compass_example.py    
```
```
    import grove_compass_lib
    c=grove_compass_lib.compass()
    while True:
            print "X:",c.x,"Y:",c.y,"X:",c.z,"Heading:",c.headingDegrees
            c.update()
            time.sleep(.1)
```

5.Run the demo.
```
    sudo python grove_compass_example.py
```

Resources
---------

-   [Grove-3-Axis Digital Compass Eagle File](assets/Grove-3-Axis_Compass_V1.0/res/Grove-3-Axis_Digital_Compass_Eagle_File.zip)
-   [HMC5883.pdf](assets/Grove-3-Axis_Compass_V1.0/res/HMC5883.pdf "File:HMC5883.pdf")
-   [Digital Compass Library](assets/Grove-3-Axis_Compass_V1.0/res/Digital_Compass.zip)


Help us make it better
-------------------------

<iframe frameborder="0" height="500" src="https://www.surveymonkey.com/r/BLGVD7F" width="500"></iframe>


<!-- 
+++
oldwikiurl       = "http://www.seeedstudio.com/wiki/Grove_-_3-Axis_Compass_V1.0"
+++
 -->

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_3-Axis_Compass_V1.0 -->