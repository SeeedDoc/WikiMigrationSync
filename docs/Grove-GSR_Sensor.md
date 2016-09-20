---
title: Grove - GSR Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-GSR-sensor-p-1614.html
oldwikiname: Grove_-_GSR_Sensor
prodimagename: GSR.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020052 1.jpg
surveyurl: https://www.research.net/r/Grove-GSR_Sensor
sku: 101020052
---

![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/GSR.jpg)

GSR, standing for galvanic skin response, is a method of measuring the electrical conductance of the skin. Strong emotion can cause stimulus to your sympathetic nervous system, resulting more sweat being secreted by the sweat glands. Grove – GSR allows you to spot such strong emotions by simple attaching two electrodes to two fingers on one hand, an interesting gear to create emotion related projects, like sleep quality monitor.


[![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/common/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-GSR-sensor-p-1614.html)

Specifications
--------------

-   Input Voltage: 5V/3.3V
-   Sensitivity adjustable via a potentiometer
-   External measuring finger cots

Demonstration
-------------

In the following we are showing you how to use the Grove - GSR.
Connect Grove - GSR Sensor to the analog port A2 of Grove-Basic Shield and Grove - Buzzer to digital port 3. ![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/GSR_Connecting.JPG)
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

![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/GSR_Result_Data.jpg)

Then take a deep breath. The buzzer should buzz now. And an obvious change in the output value should be observed.
The below is a graphs which is created in Excel using the data above. X axis represents time. and Y axis GSR data.

![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/Result_Chart.jpg)

Reference
---------

There are several graphs which are created in excel using GSR data.You can open the [GSR sensor data.xls](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/res/GSR_sensor_data.xls) to see the detail data.
![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/Reference_graphs1.png)![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/Reference_graphs3.png)
![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/Reference_graphs2.png)![](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/img/Reference_graphs4.png)

Resources
---------

- [Grove - GSR Eagle File](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/res/Grove-GSR_Eagle_File.zip)
- [LM324 datasheet](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/res/Lm324.pdf)
- [GSR sensor data.xls](https://github.com/SeeedDoc/WikiMigrationSync/raw/master/docs/assets/Grove-GSR_Sensor/res/GSR_sensor_data.xls "File:GSR sensor data.xls")

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_GSR_Sensor -->
