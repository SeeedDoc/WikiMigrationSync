<!-- 
+++
title       = "Grove - I2C Touch Sensor"
+++
 -->

# Grove - I2C Touch Sensor

![](/assets/Grove-I2C_Touch_Sensor/img/Grove-I2C-Touch-Sensor.jpg)

Introduction
------------

The I2C Touch Sensor is based on the Proximity Capacitive Touch Sensor Controller from FreeScale - MPR121. It detects the touch or proximity of human fingers. This sensor includes a Touch Sensor controller and 4 finger feelers. One can insert the connectors of feelers into base of Sensor controller, and start sensing the touch. 

[![](/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/depot/Grove-I2C-Touch-Sensor-p-840.html)

Specifications
-------------

| Parameter              | Value/Range                         |
|------------------------|-------------------------------------|
| Operating voltage      | 3~5.5V                              |
| Standby Mode Current   | 2μA                                 |
| Touch Channels         | 12 (Including 4 with Touch feelers) |
| Communicating Protocol | I2C                                 |
| I2C Address            | 0x5A - 0x5D                         |

Hardware Overview
-----------------

![](/assets/Grove-I2C_Touch_Sensor/img/DSC_0030.png)

There are 12 electrodes CH0-CH11. CH0-CH3 are connected to 4 Touch feelers.

The CH4-CH11 are for customer expanding the function. If you need more, you can make the feelers by yourself.

The wires of feelers are twisted to reduce the impact of environment. The black(ground) wire can be cut off if high sensitivity is needed.

The INT pin has to be led out if customers want to use the interrupt pin of MPR121.

Getting Started
---------------

### **Grove - Help**

Following documents help in getting the user started with Grove.

-   [Preface - Getting Started](http://www.seeedstudio.com/document/pdf/Preface.pdf)
-   [Introduction to Grove](http://www.seeedstudio.com/document/pdf/Introduction%20to%20Grove.pdf)

<div class="admonition note">
<p class="admonition-title">Note</p>
Since each electrode needs to be auto-configured by the MPR121 during power up and there is no power reset on the touch sensor controller, everytime you insert or remove a feeler, you need to reset the power of Seeeduino.
</div>

The feelers can also feel the human being fingers with something between, that's to say, you do not need to touch the feelers with your fingers indeed.

![](/assets/Grove-I2C_Touch_Sensor/img/DSC_0026.jpg)

![](/assets/Grove-I2C_Touch_Sensor/img/DSC_0027.jpg)

With a paperboard about 3 mm thick, the feeler can feel the touch of fingers, makes it a good solution for many applications.

Resources
---------

-   [I2C Touch Sensor Library](https://github.com/Seeed-Studio/Grove_I2C_Touch_Sensor)
-   [I2C Touch Sensor eagle files(v1.1).zip](/assets/Grove-I2C_Touch_Sensor/res/I2C_Touch_Sensor_eagle_files-v1.1-.zip)
-   [I2C Touch Sensor PDF](/assets/Grove-I2C_Touch_Sensor/res/Grove-I2C_Color_sensor_v1.2.pdf)
-   [How to detect finger touch?](/How_to_detect_finger_touch?)
-   [I2C Touch Sensor Datasheet](/assets/Grove-I2C_Touch_Sensor/res/Freescale_Semiconductor;MPR121QR2.pdf)

Help us make it better
-------------------------

<iframe frameborder="0" height="500" src="https://www.surveymonkey.com/r/RDQDY53" width="500"></iframe>


<!-- 
+++
oldwikiurl       = "http://www.seeedstudio.com/wiki/Grove_-_I2C_Touch_Sensor"
+++
 -->

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_I2C_Touch_Sensor -->