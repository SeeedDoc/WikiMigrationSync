<!-- 
+++
title       = "EL Shield"
+++
 -->

# EL Shield

![](/assets/EL_Shield/img/EL_Shield_02.jpg)

Introduction
------------

This shield is used to control EL devices. It can control 4 EL devices simultaneously. The controlling method is as simple as controlling an LED. Driven by PWM, it can create a colorful and florid effect by controlling each EL wire with a simple program. Combined with our EL Inverter, it can drive an EL wire as long as 15m, which provides infinite possibility for your design. Besides, the Shield is covered by Acrylic board, which enhances user's safety.

[![](/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/el-shield-p-1287.html)

Specifications
--------------

- Operating Voltage: 5V
- Invertor interface: JST 2.0
- Control channel interface: 2P - 2.5SM socket

Hardware Overview
---------

![](/assets/EL_Shield/img/EL_Shield_interface.jpg)

Demonstration
-------------

Here is a simple demo involving EL shield, 4 EL tapes and the custom invertor that accompanies EL shield.
Hook all things up as in the picture below.

![](/assets/EL_Shield/img/EL_Shield_Hardware_Installation.jpg)

Upload the code below to your microcontroller.

```
// EL test code 
 
void setup(){
 for(int i = 4; i<8; i++)
 { 
  pinMode(i, OUTPUT);
 }
}
 
void setEL(int ch) // set a certain EL on
{ 
 for(int i = 4; i<8; i++) // all off
 digitalWrite(i, LOW);
 digitalWrite(ch+3, HIGH); // ch on
} 
 
int count = 0; 
 
void loop()
{ 
 setEL(count%4 + 1);
 delay(200);
 if(count++ == 1000)
 { 
  count = 0;
 } 
}
```

Resources
---------

-   [EL Shield eagle file](/assets/EL_Shield/res/EL_Shield_Eagle_File.zip)
-   [EL Shield Source code file for Arduino 1.0](/assets/EL_Shield/res/EL_Shield_Test_code.zip)
-   [BT134W-600D datasheet](/assets/EL_Shield/res/BT134W-600D.pdf)
-   [MOC 3063 datasheet](/assets/EL_Shield/res/MOC3063M.pdf)


Help us make it better
-------------------------

<iframe frameborder="0" height="500" src="https://www.surveymonkey.com/r/3XGX9ZC" width="500"></iframe>

<!-- 
+++
oldwikiurl       = "http://www.seeedstudio.com/wiki/EL_Shield"
+++
 -->

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/EL_Shield -->
