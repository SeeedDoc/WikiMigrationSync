---
title: Grove - Fingerprint Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Fingerprint-Sensor-p-1424.html
oldwikiname: Grove_-_Fingerprint_Sensor
prodimagename: Print_Sensor.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/Print Sensor.jpg
surveyurl: https://www.research.net/r/Grove-Fingerprint_Sensor
sku: 101020057
---

![](assets/Grove-Fingerprint_Sensor/img/Print_Sensor.jpg)

The Finger Print Sensor is one optical fingerprint sensor which will make fingerprint detection and verification adding super simple.There's a high powered DSP chip AS601 that does the image rendering, calculation, feature-finding and searching. You can also enroll new fingers directly - up to 162 finger prints can be stored in the onboard FLASH memory. There's a red LED in the lens which will light up during taking photos so that you know its working condition. It is easy to use and by far the best fingerprint sensor you can get.

[![](assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Fingerprint-Sensor-p-1424.html)

Specifications
-------------

-   Supply voltage: 3.6~6.0 V
-   Operating current(Max) : 120 mA
-   Fingerprint imaging time: 1.0 S
-   Match Mode: Compare Mode 1:1
-   Search Mode: 1:N
-   Storage capacity: 162 templates
-   False Acceptance Rate : 0.001% (Security level 3)
-   False Reject Rate ：1.0% (Security level 3)
-   Baud rate ：9600, 19200, 28800, 38400, 57600bps (default is 57600)
-   Interface：TTL Serial
-   Work Temperature：-20 ~ +50 ℃
-   Interface

| Pin Number | Name | Type | Function Description                                     |
|------------|------|------|----------------------------------------------------------|
| 1          | Vin  | in   | Positive Power Supply Input Terminal(Line color:Red)     |
| 2          | TD   | out  | Serial data output, TTL logic levels(Line color: Yellow) |
| 3          | RD   | in   | Serial data input, TTL logic levels(Line color: White)   |
| 4          | GND  | -    | Signal ground(Line color: Black)                         |

Demonstration
-------------

The Finger Print Sensor module is typically used in safes - there's a high powered DSP chip that does the image rendering, calculation, feature-finding and searching. Connect to any microcontroller or system with TTL serial, and send packets of data to take photos, detect prints, hash and search. You can also enroll new fingers directly - up to 162 finger prints that can be stored in the onboard FLASH memory. There's a red LED in the lens which will light up during taking photos so that you know its working condition.

-   Connect the Sensor to the Digital Port 2 of the [Grove - Base Shield](/Grove-Base_Shield "Grove - Base Shield").
-   Plug the Grove - Base Shield into Arduino and connect Arduino to PC by using a USB cable.

When you plug in the power, you can see the red LED blink which indicates the sensor is working.

![](assets/Grove-Fingerprint_Sensor/img/FingerPrint_Sensor1.jpg)

-   Download the [Finger Print Sensor Library](assets/Grove-Fingerprint_Sensor/res/Fingerprint_library.rar) and Unzip it into the libraries file of Arduino IDE by the path: ..\\arduino-1.0.1\\libraries.

The library can enroll and search so its perfect for any project. It can help you get running in under 10 minutes. There are basically two requirements for using the optical fingerprint sensor. First one, you'll need to enroll fingerprints - that means assigning ID \#'s to each print so you can query them later. Once you've enrolled all your prints, you can easily 'search' the sensor, asking it to identify which ID (if any) has currently been photographed.

-   Open the enroll code directly by the path: File->Example->FingerPrint->Enroll.
-   Upload the code into Arduino. Please click [here](/Upload_Code) if you do not know how to upload.
-   Start up Serial Tool and Select the ComNum and BaudRate used by the Arduino.
-   Select the "SendNew" option. Send the ID \# you want to use. You can use up to 162 ID numbers. And it will ask you to press the finger to the sensor. At the moment, you should see the red LED blink.

![](assets/Grove-Fingerprint_Sensor/img/FingerPrint_Sensor3.jpg)
![](assets/Grove-Fingerprint_Sensor/img/Finger1.jpg)

-   If your press is OK, you could see the following message. You will then have to repeat the process, to get a second clean print. Use the same finger! On success you will see the message.


![](assets/Grove-Fingerprint_Sensor/img/Finger2.jpg)

-   If there's a problem such as a bad print or image, you'll have to do it again.

![](assets/Grove-Fingerprint_Sensor/img/Finger_Print_Score_2.jpg)

Once you have the finger enrolled, it's a good idea to do a quick test to make sure it can be found in the database.

-   Open the demo code:fingerprint and upload it.
-   When prompted, press a different/same finger to the sensor. If it is the same finger, you should get a match with the ID \# as show below.

![](assets/Grove-Fingerprint_Sensor/img/Finger_Print_Score_3.jpg)

-   If it is not a finger in the database, This serial port will output nothing.

Resources
--------

- [Finger Print Sensor Library File](assets/Grove-Fingerprint_Sensor/res/Fingerprint_library.rar)
- [Finger Print Sensor Datasheet](assets/Grove-Fingerprint_Sensor/res/ZFM206用户手册V2.1.pdf)

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Fingerprint_Sensor -->