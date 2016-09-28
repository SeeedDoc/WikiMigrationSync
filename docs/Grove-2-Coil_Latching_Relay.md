---
title: Grove - 2-Coil Latching Relay
category: Actuator
bzurl: https://seeedstudio.com/Grove-2-Coil-Latching-Relay-p-1446.html
oldwikiname: Grove_-_2-Coil_Latching_Relay
prodimagename: 2Coil_Latching_Relay_01.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/2Coil Latching Relay.jpg
surveyurl: https://www.research.net/r/Grove-2-Coil_Latching_Relay
sku: 103020010
tags: grove_digital, io_5v, plat_duino
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-2-Coil_Latching_Relay/master/img/2Coil_Latching_Relay_01.jpg)

This module is based on 2-Coil Latching Relay. Contrast to the ordinary relay, this latching relay does not need continuous power to keep the state, only a rising/falling pulse is needed to change the work state. Even the power can be removed when the work state do not need to change, making this module especially suitable for low-power projects.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-2-Coil-Latching-Relay-p-1446.html)

Features
-------

-   Grove Connector
-   Low power consumption
-   Dual Switch

Specifications
-------------

<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
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
<th scope="row">
Working Voltage
</th>
<td>
4.7
</td>
<td>
5.0
</td>
<td>
5.3
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th scope="row">
Set/Reset Voltage(Max)
</th>
<td colspan="3">
4.0
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th scope="row">
Coil Resistance
</th>
<td>
151
</td>
<td>
167
</td>
<td>
183
</td>
<td>
Ω
</td>
</tr>
<tr align="center">
<th scope="row">
Switching Voltage(Max)
</th>
<td colspan="3">
35VAC/35VDC
</td>
<td>
/
</td>
</tr>
<tr align="center">
<th scope="row">
Switching Current(Max)
</th>
<td colspan="3">
3
</td>
<td>
A
</td>
</tr>
<tr align="center">
<th scope="row">
Set Time(Latching)
</th>
<td colspan="3">
4.5(max)
</td>
<td>
ms
</td>
</tr>
<tr align="center">
<th scope="row">
Reset Time(Latching)
</th>
<td colspan="3">
3.5(max)
</td>
<td>
ms
</td>
</tr>
</table>

Platforms Supported
-------------------

Usage
-----

### With Arduino

The latching relay only draws power during the changing of state. A rising/falling voltage pulse on the signal pin changes it's working state. This is very useful in situations where energy efficiency is important, and also in situations where you need the relay to remember its state.

Let's begin to use it.

-   Connect the module to D3 port of [Grove - Base Shield](/Grove-Base_Shield "Grove - Base Shield").
-   The relay hold in "set" status(Comm and NO connected) in default, when there is a rising edge on the SIG pin. It turns the "reset" state(Comm and NC connected). The reference code is shown below:

```
    #define LatchingRelay 3
    void setup()
    {
    pinMode(LatchingRelay,OUTPUT);

    digitalWrite(LatchingRelay,LOW);
    delay(1000);
    digitalWrite(LatchingRelay,HIGH);
    delay(1000);

    }
    void loop()
    {

    }
```

-   The relay hold in "reset" status(Comm and NC Connected), when there is a falling edge on the SIG pin. It turns the "set" state(Comm and NO connected). The reference code is shown below:

```
    #define LatchingRelay 3
    void setup()
    {
    pinMode(LatchingRelay,OUTPUT);

    digitalWrite(3,HIGH);
    delay(1000);
    digitalWrite(3,LOW);
    delay(1000);
    }
    void loop()
    {

    }
```

-   This module consumes little power when working state doesn't change. After setting the relay state, you do not need to supply power for the Latching Relay any more, which makes it especially low power consumption.

<div class="admonition note">
<p class="admonition-title">Note</p>
Relay is on the "reset" status when being released from stock.
</div>

![](https://raw.githubusercontent.com/SeeedDocument/Grove-2-Coil_Latching_Relay/master/img/Latching_Relay_Diagram.jpg)


<div class="admonition note">
<p class="admonition-title">Notes</p>
<p> 1. The two-way relays are controlled at the same time.</p>
<p> 2. The NO(NC) indicator will flash once when switch to "set"("reset") status.</p>
</div>


### With [Raspberry Pi](/GrovePiPlus "GrovePi+")

1.You should have got a raspberry pi and a grovepi or grovepi+.

2.You should have completed configuring the development enviroment, otherwise follow [here](/GrovePiPlus#Introducing_the_GrovePi.2B).

3.Connection

-   Plug the sensor to grovepi socket D4 by using a grove cable.

4.Navigate to the demos' directory:

```
    cd yourpath/GrovePi/Software/Python/
```
-   To see the code

```
    nano grove_2_coil_latching_relay.py   # "Ctrl+x" to exit #
```

```
    import time
    import grovepi

    # Connect the Grove 2-Coil Latching Relay to digital port D4
    # SIG,NC,VCC,GND
    relay = 4

    grovepi.pinMode(relay,"OUTPUT")

    while True:
        try:
            # switch on for 5 seconds
            grovepi.digitalWrite(relay,1)
            print "on"
            time.sleep(5)

            # switch off for 5 seconds
            grovepi.digitalWrite(relay,0)
            print "off"
            time.sleep(5)

        except KeyboardInterrupt:
            grovepi.digitalWrite(relay,0)
            break
        except IOError:
            print "Error"

```

5.Run the demo.
```
    sudo python grove_2_coil_latching_relay.py
```

Resources
--------

- [Grove - 2-Coil Latching Relay Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-2-Coil_Latching_Relay/master/res/Grove-2-Coil_Latching_Relay_Eagle_File.zip)
- [Latching_Relay_Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-2-Coil_Latching_Relay/master/res/Latching_Relay_Datesheet.pdf)

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_2-Coil_Latching_Relay -->
