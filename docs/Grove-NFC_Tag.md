<!-- 
+++
title       = "Grove - NFC Tag"
+++
 -->

# Grove - NFC Tag

![](/assets/Grove-NFC_Tag/img/Grove-NFC_Tag_uasge.jpg)

Introduction
------------


Grove - NFC Tag is a highly integrated Near Field Communication Tag module,this module is I2C interface,which base on M24LR64E-R,M24LR64E-R have a 64-bit unique identifier and 64 -Kbit EEPROM.Grove - NFC Tag attach an independent PCB antenna which can easily stretch out of any enclosure you use, leaving more room for you to design the exterior of your project.


[![](/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-NFC-Tag-p-1866.html)

Specifications
=============

-   Working Voltage:5V or 3V3
-   Working Current&lt;1mA
-   Effective range&lt;2cm
-   Serve for contactless communication at 13.56MHz
-   ISO 15693 and ISO 18000-3 mode 1 compatible
-   64-bit unique identifier (UID)
-   Read Block & Write (32-bit blocks)
-   Grove I2C Interface

Usage
=====

Read/Write from Mobile
--------------------

1.  Download [NfcV-reader for Android](https://github.com/Seeed-Studio/NFC_Tag_M24LR6E/blob/master/Resources/NfcVreader.apk) and install it
2.  We can Read/Write it from Mobile

![](/assets/Grove-NFC_Tag/img/NFC_Tag_1.png)

![](/assets/Grove-NFC_Tag/img/NFC_Tag_2.jpg)

![](/assets/Grove-NFC_Tag/img/NFC_Tag_3.jpg)

![](/assets/Grove-NFC_Tag/img/NFC_Tag_4.png)

Control LED
-----------

1.  Hardware Installation

![](/assets/Grove-NFC_Tag/img/Grove-NFC_Tag_Photo.jpg)

1.  Download [NfcV-reader for Android](https://github.com/Seeed-Studio/NFC_Tag_M24LR6E/blob/master/Resources/NfcVreader.apk) and install it
2.  Download [NFC Tag Lib](https://github.com/Seeed-Studio/NFC_Tag_M24LR6E), rename it to NFC_Tag_M24LR6E and put it into Arduino's library .
3.  Open Arduino IDE. If Arduino IDE is already opened, restart it.
4.  In Arduino IDE, click menus: File -> Example -> NFC_Tag_M24LR6E -> ledControl
5.  Now, you can control LED from your phone.

```
 
#include "NfcTag.h"
#include <Wire.h>
 
NfcTag nfcTag;
int led = 5;
bool flag = false;
bool preFlag = false;
void setup(){
  Serial.begin(9600);
  pinMode(led,OUTPUT);
  nfcTag.init();
}
 
void loop(){
  flag = nfcTag.readByte(EEPROM_I2C_LENGTH-1) == 0xff?true:false;
  if(flag != preFlag){
    Serial.println("get remote NFC control signal!");
    if(flag == true){
      Serial.println("led will light up!");
      digitalWrite(led,HIGH);
    }else{
      Serial.println("led will turn dark!");
      digitalWrite(led,LOW);
    }
    preFlag = flag;
  }
  delay(5*1000);
}
```

Resources
--------

-   [Grove - NFC Tag.PDF](/assets/Grove-NFC_Tag/res/Grove-NFC_Tag_v1.0.pdf)
-   [Grove - NFC Tag Eagle file](/assets/Grove-NFC_Tag/res/Grove-NFC_Tag_v1.0.zip)
-   [M24LR64E-R datasheet.pdf](/assets/Grove-NFC_Tag/res/M24LR64E-R.pdf)
-   [NfcV-reader for Android](https://github.com/Seeed-Studio/NFC_Tag_M24LR6E/blob/master/Resources/NfcVreader.apk)
-   [NFC Tag M24LR6E Lib](https://github.com/Seeed-Studio/NFC_Tag_M24LR6E)



Help us make it better
-------------------------

<iframe frameborder="0" height="500" src="https://www.surveymonkey.com/r/KN5M2NH" width="500"></iframe>

<!-- 
+++
oldwikiurl       = "http://www.seeedstudio.com/wiki/Grove_-_NFC_Tag"
+++
 -->

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_NFC_Tag -->
