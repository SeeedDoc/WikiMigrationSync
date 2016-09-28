---
title: Grove - 6-Axis Accelerometer&Gyroscope
category: Sensor
bzurl: https://seeedstudio.com/Grove-6-Axis-Accelerometer&Gyroscope-p-2606.html
oldwikiname: Grove_-_6-Axis_Accelerometer&Gyroscope
prodimagename: Grove-6-Axis_AccelerometerAndGyroscope_product_view_1200_s.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/105020012 3.jpg
surveyurl: https://www.research.net/r/Grove-6-Axis_AccelerometerAndGyroscope
sku: 105020012
tags: plat_duino, plat_pi, plat_bbg, plat_linkit -->
---

<!-- tags: io_3v3, io_5v, grove_i2c, grove_analog, grove_digital, grove_uart, plat_duino, plat_bbg, plat_pi, plat_wio, plat_linkit -->

![](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/img/Grove-6-Axis_AccelerometerAndGyroscope_product_view_1200_s.jpg)

Grove - 6-Axis Accelerometer&Gyroscope is a cost-effective Grove interfaced and integrated sensor combination of 3-axis digital accelerometer and 3-axis digital gyroscope.

With a serious low power consumption digital chip LSM6DS3([datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/res/LSM6DS3TR.pdf)) and power supply regulator inside, it features high sensitivity, green tech and low noise interference. It can be configured to different sensitivity levels of acceleration and different angular rate measurement range. Provided with detailed SDK, it can make the prototyping process quicker and easier.

This product can be used for different applications for tilt, motion, and tap sensings, such as robotics, IoT devices and consumer electronic devices.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-6-Axis-Accelerometer&Gyroscope-p-2606.html)

Features
--------

-   Grove interfaced and cost-effective.
-   Digital-output for 6 DOF motion data.
-   ±2/±4/±8/±16 g full scale leaner acceleration sensing range for various environment.
-   ±125, ±245, ±500, ±1000, ±2000 degree per seconds(dps) for angular rate measurement range make it versatile.
-   Detailed SDK for easier programming.
-   Regulated power supply for reliable data to be collected.
-   Programmed interrupts for different event.
-   8 kB data buffering.


Application ideas
-----------------

-   Robotics
-   Consumer-level aircraft
-   Computer input devices
-   Wearable devices.
-   IoT things

Specifications
--------------

For detailed information please refer to [datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/res/LSM6DS3TR.pdf).

| Parameter                             | Value                                                                                |
|---------------------------------------|--------------------------------------------------------------------------------------|
| Analog supply voltage:                | 5V/3.3V(DC)                                                                          |
| Power consumption:                    | 0.9 mA in combo normal mode and 1.25 mA in combo high-performance mode up to 1.6 kHz |
| Linear acceleration measurement range | ±2/±4/±8/±16 g full scale (typical value)                                            |
| Angular rate measurement range        | ±125, ±245, ±500, ±1000, ±2000 dps(typical value)                                    |
| Linear acceleration sensitivity       | 0.061(FS = ±2), 0.122(FS = ±4), 0.244(FS = ±8), 0.488(FS = ±16) mg/LSB               |
| Angular rate sensitivity              | 4.375(FS = ±125), 8.75(FS = ±245), 17.50(FS = ±500), 35(FS = ±1000), 70(FS = ±2000)  |

### Platforms Supported

<div class="admonition note">
<p class="admonition-title">Note</p>
If no version number is not represented for a specific platform, it means this product support all versions within this platform. But you will need additional corresponding Grove shield board such as Grove - Base Shield v2.
</div>

Hardware Overview
-----------------

![](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/img/Grove-6-Axis_AccelerometerAndGyroscope_components_view_1200_s.jpg)

**Grove Port**   
Connect main control board such as Seeeduino board with driver board.

**LSM6DS3**   
Main MCU.

### **Parts list**

| Parts name                             | Quantity |
|----------------------------------------|----------|
| Grove - 6-Axis Accelerometer&Gyroscope | 1PC      |
| Grove wire                             | 1PC      |

Get started
-----------

### **Material required**

-   Seeeduino * 1

-   Grove - Base Shield v2

### **Preparations**

Refer to following guides to build an appropriate IDE:

<div class="admonition note">
<p class="admonition-title">Note</p>
We have chosen Seeeduino and it is compatible with Arduino in this case. You can also use Arduino board instead.
</div>

[Getting Started on Windows](/Seeeduino_v4.2#Getting_Started_on_Windows)

[Getting Started on Mac OS X](/Seeeduino_v4.2#Getting_Started_on_Mac_OS_X)

### **Hardware connections**

![](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/img/Grove-6-Axis_AccelerometerAndGyroscope_demo_connection_1200_s.jpg)

<div class="admonition note">
<p class="admonition-title">Note</p>
Plug Grove - 6-Axis Accelerometer&Gyroscope to I<sup>2</sup>C interface on Grove - Base shield. Connect power supply with USB cable.
</div>

### **A little demo**

Download the [library](https://github.com/Seeed-Studio/Accelerometer_And_Gyroscope_LSM6DS3) for Grove - 6-Axis Accelerometer&Gyroscope. Refer to [Guide to use demos downloaded from Seeed's Github](/Guide_to_use_demos_downloaded_from_Seeed's_Github) for quicker flashing your code to main controller board. There are three demo examples in total in sub directory ***examples***.

Resources
---------

-   [Schematic files](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/res/Schematic_files.zip)
-   [Github](https://github.com/Seeed-Studio/Accelerometer_And_Gyroscope_LSM6DS3)
-   [Datasheet of LSM6DS3](https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/res/LSM6DS3TR.pdf)


<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_6-Axis_Accelerometer&Gyroscope -->
