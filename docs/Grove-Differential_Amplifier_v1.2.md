---
title: Grove - Differential Amplifier v1.2
category: Others
bzurl: https://www.seeedstudio.com/Grove-Differential-Amplifier-p-1284.html
oldwikiname: Grove_-_Differential_Amplifier_v1.2
prodimagename: Grove-Differential_Amplifier_v1.2.jpg
bzprodimageurl: https://statics3.seeedstudio.com/images/103020016 1.jpg
surveyurl: https://www.research.net/r/Grove-Differential_Amplifier_v1.2
sku: 103020016
---

![](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-Differential_Amplifier_v1.2/img/Grove-Differential_Amplifier_v1.2.jpg)

This Grove is designed for precise differential-input amplification. Input the differential signals of your sensor to this module through the male pins, then your Arduino will get a precisely amplified output from the Grove interface. The gain scale factor is selectable. You can get a 35 times or 1085 times amplification via a switch on the board. 

[![](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Differential-Amplifier-p-1284.html)


Features
-------

-   High amplifying precision
-   Selectable scale factor
-   Can be conveniently read by Arduino

Applications
-----------

-   Data acquisition
-   Battery operated systems
-   Pressure and temperature bridge amplifiers
-   General purpose instrumentation

Specifications
-------------

<table border="1" cellspacing="0" width="80%">
<tr>
<th colspan="2" scope="col">
Item
</th>
<th scope="col">
Min
</th>
<th scope="col">
Typical
</th>
<th scope="col">
Max
</th>
<th scope="col">
Unit
</th>
</tr>
<tr align="center">
<th colspan="2" scope="row">
Operating Voltage
</th>
<td>
2.7
</td>
<td>
5.0
</td>
<td>
5.5
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th colspan="2" scope="row">
Input Voltage
</th>
<td>
0.1
</td>
<td>
\\
</td>
<td>
(Vcc-0.8)/Gain
</td>
<td>
mV
</td>
</tr>
<tr align="center">
<th colspan="2" scope="row">
Output Voltage
</th>
<td>
0
</td>
<td>
\\
</td>
<td>
Vcc-0.80
</td>
<td>
mV
</td>
</tr>
<tr align="center">
<th rowspan="2">
Gain
</th>
<td>
Select 35
</td>
<td>
/
</td>
<td>
35
</td>
<td>
/
</td>
<td colspan="2" rowspan="2">
/
</td>
</tr>
<tr align="center">
<td>
Select 1085
</td>
<td>
/
</td>
<td>
1085
</td>
<td>
/
</td>
</tr>
</table>
Usage
-----

**1. Sensor Choosing**

The amplifier can turn signals in mA scale up to A scale. Before using it, make sure the output range of your sensor is in mA scale. For example, [Weight Sensor](/Weight_Sensor-Load_Cell-0-500g) is one of them.

**2. Connector Reforming**

To pair the weight sensor up with the male pins on the amplifier, female connectors need to be soldered on its wires.

![](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-Differential_Amplifier_v1.2/img/Solder.jpg)

**3. Hardware Hookup**

Connect the weight sensor to the amplifier as the picture depicts below.

![](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-Differential_Amplifier_v1.2/img/Connect5.jpg)

**4. Measurement**

Copy and paste the demo code below to Arduino IDE and upload it.

```
    void setup()
    {
      Serial.begin(9600);
      Serial.println("start");
    }

    void loop()
    {
      int i;
      int value;
      float V,Vo;
      float Sum=0;
      for(i=0;i<10;i++)
      {
        value=analogRead(4);
        V=value*5.00/1023;
        Sum+=V;
        delay(10);
      }
      Vo=Sum/10;
      Serial.print("Output score:");
      Serial.println(Vo);
      delay(1000);
    } 
```

You can view the amplified signals via serial monitor. For the value of the input signal, you need to use the multimeter to measure the voltage difference between VIN+ and VIN-.

Resources
--------

- [v1.2 Eagle File](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-Differential_Amplifier_v1.2/res/Grove-Differential_Amplifier_v1.2_eagle.zip)
- [v1.2 Schematic](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-Differential_Amplifier_v1.2/res/Grove-Differential_Amplifier_v1.2.pdf)
- [INA132 Datasheet](/https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-Differential_Amplifier_v1.2/res/Ina132.pdf)

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Differential_Amplifier_v1.2 -->
