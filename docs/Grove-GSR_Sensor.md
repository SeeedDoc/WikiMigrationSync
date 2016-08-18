<!-- 
+++
title       = "Grove - GSR Sensor"
+++
 -->

# Grove - GSR Sensor

![](/assets/Grove-GSR_Sensor/img/GSR.jpg)

Introduction
------------

GSR, standing for galvanic skin response, is a method of measuring the electrical conductance of the skin. Strong emotion can cause stimulus to your sympathetic nervous system, resulting more sweat being secreted by the sweat glands. Grove – GSR allows you to spot such strong emotions by simple attaching two electrodes to two fingers on one hand, an interesting gear to create emotion related projects, like sleep quality monitor.


[![](/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-GSR-sensor-p-1614.html)

Specifications
--------------

-   Input Voltage: 5V/3.3V
-   Sensitivity adjustable via a potentiometer
-   External measuring finger cots

Demonstration
-------------

In the following we are showing you how to use the Grove - GSR.
Connect Grove - GSR Sensor to the analog port A2 of Grove-Basic Shield and Grove - Buzzer to digital port 3. ![](/assets/Grove-GSR_Sensor/img/GSR_Connecting.JPG)
Copy and paste the code below to a new Arduino sketch and upload it to Arduino.

    const int BUZZER=3;
    const int GSR=A2;
    int threshold=0;
    int sensorValue;

    void setup(){
      long sum=0;
      Serial.begin(9600);
      pinMode(BUZZER,OUTPUT);
      digitalWrite(BUZZER,LOW);
      delay(1000);
      
      for(int i=0;i<500;i++)
      {
      sensorValue=analogRead(GSR);
      sum += sensorValue;
      delay(5);
      }
      threshold = sum/500;
       Serial.print("threshold =");
       Serial.println(threshold);
      }

    void loop(){
      int temp;
      sensorValue=analogRead(GSR);
      Serial.print("sensorValue=");
      Serial.println(sensorValue);
      temp = threshold - sensorValue;
      if(abs(temp)>50)
      {
        sensorValue=analogRead(GSR);
        temp = threshold - sensorValue;
        if(abs(temp)>50){
        digitalWrite(BUZZER,HIGH);
        Serial.println("YES!");
        delay(3000);
        digitalWrite(BUZZER,LOW);
        delay(1000);}
      }
      }

Wear the finger sheath and relax, Now open serial monitor, we can see:

![](/assets/Grove-GSR_Sensor/img/GSR_Result_Data.jpg)

Then take a deep breath. The buzzer should buzz now. And an obvious change in the output value should be observed.
The below is a graphs which is created in Excel using the data above. X axis represents time. and Y axis GSR data.

![](/assets/Grove-GSR_Sensor/img/Result_Chart.jpg)

Reference
---------

There are several graphs which are created in excel using GSR data.You can open the [GSR sensor data.xls](/assets/Grove-GSR_Sensor/res/GSR_sensor_data.xls) to see the detail data.
![](/assets/Grove-GSR_Sensor/img/Reference_graphs1.png)![](/assets/Grove-GSR_Sensor/img/Reference_graphs3.png)
![](/assets/Grove-GSR_Sensor/img/Reference_graphs2.png)![](/assets/Grove-GSR_Sensor/img/Reference_graphs4.png)

Resources
---------

- [Grove - GSR Eagle File](/assets/Grove-GSR_Sensor/res/Grove-GSR_Eagle_File.zip)
- [LM324 datasheet](/assets/Grove-GSR_Sensor/res/Lm324.pdf)
- [GSR sensor data.xls](/assets/Grove-GSR_Sensor/res/GSR_sensor_data.xls "File:GSR sensor data.xls")

Help us make it better
-------------------------

<iframe frameborder="0" height="500" src="https://www.surveymonkey.com/r/KJP2KGB" width="500"></iframe>


<!-- 
+++
oldwikiurl       = "http://www.seeedstudio.com/wiki/Grove_-_GSR_Sensor"
+++
 -->

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_GSR_Sensor -->
