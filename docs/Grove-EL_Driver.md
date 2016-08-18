<!-- 
+++
title       = "Grove - EL Driver"
+++
 -->

# Grove - EL Driver

![](/assets/Grove-EL_Driver/img/Grove-EL_Driver.jpg)

Introduction
------------

Grove - EL Driver is designed for driving EL Wires. It integrates a very small inverter to drive the EL Wire, so you can easily light up the EL Wire with just one single Grove cable.


[![](/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-EL-Driver-p-2269.html)

Version Tracker
---------------

| Revision | Descriptions           | Release      |
|----------|------------------------|--------------|
| v1.0     | Initial public release | Dec 11, 2014 |


#### **Supported EL Wires:**

-   [EL Wire-Green 3m](http://www.seeedstudio.com/depot/EL-WireGreen-3m-p-1102.html)
-   [EL Wire-Red 3m](http://www.seeedstudio.com/depot/EL-WireRed-3m-p-1129.html)
-   [EL Wire-Blue 3m](http://www.seeedstudio.com/depot/EL-WireBlue-3m-p-1128.html)
-   [EL Wire-Yellow 3m](http://www.seeedstudio.com/depot/EL-WireYellow-3m-p-1127.html)
-   [EL Wire-White 3m](http://www.seeedstudio.com/depot/EL-WireWhite-3m-p-1130.html)

Features
--------

-   Grove compatible interface
-   3.3V/5V Compatible
-   Integrated Inverter Transformer
-   Input Current: 300mA Max (According to the load)
-   Supported max EL Capacitance: 15nF

Usage
-----

Here we show how to use Arduino to control the state of the LED.

1. Connect the Grove - EL Driver to Base Shield's **digital port 2** with 4pin Grove Cable. Of course you can change to other valid digital ports if it's necessary and the definitions of the port should be changed too. Connect a EL Wire to EL Driver **J1** port with the given cable in product package.

2. Plug it onto the Arduino/Seeeduino. Connect the board to PC using USB cable.

3. Copy the demo code to your sketch, then upload to Arudino or Seeeduino board. Please click [here](/Upload_Code) if you do not know how to upload.
You will see the EL Wire blink every second.

```
/*************************   2014 Seeedstudio   **************************
* File Name          : GroveELDriverDemoCode.ino
* Author             : Seeedteam
* Version            : V1.0
* Date               : 11/12/2014
* Description        : Demo code for Grove - EL Driver
*************************************************************************/
 
#define ELPin 2 //connect EL Driver to digital pin2
void setup() {                
  // initialize the digital pin2 as an output.
  pinMode(ELPin, OUTPUT);     
}
 
void loop() {
  digitalWrite(ELPin, HIGH);   // set the EL Wire on
  delay(500);               // for 500ms
  digitalWrite(ELPin, LOW);   // set the EL Wire off
  delay(500);
}
```

![](/assets/Grove-EL_Driver/img/Grove-EL_Driver_usage.jpg)

Resources
---------

-   [sch_pcb_eagle](/assets/Grove-EL_Driver/res/Grove-EL_Driver_v1.0.zip)
-   [sch_pdf](/assets/Grove-EL_Driver/res/Grove-EL_Driver_v1.0.pdf)


Help us make it better
-------------------------

<iframe frameborder="0" height="500" src="https://www.surveymonkey.com/r/GLY6YXP" width="500"></iframe>


<!-- 
+++
oldwikiurl       = "http://www.seeedstudio.com/wiki/Grove_-_EL_Driver"
+++
 -->

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_EL_Driver -->
