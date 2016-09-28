---
title: Seeeduino Cloud and Grove IoT Starter Kit Powered by AWS
category: Arduino
bzurl: https://www.amazon.com/Seeeduino-Cloud-Grove-Starter-Powered/dp/B01669BB60
oldwikiname: Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS
prodimagename: Aws_seeeduino_wiki_cover.JPG
bzprodimageurl: https://images-na.ssl-images-amazon.com/images/I/71NtWHsITmL._SL1500_.jpg
surveyurl: https://www.research.net/r/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS
---
<!-- tags: io_3v3, io_5v, grove_i2c, grove_analog, grove_digital, grove_uart, plat_duino, plat_bbg, plat_pi, plat_wio, plat_linkit -->

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Aws_seeeduino_wiki_cover.JPG)

*Main articles: Start here [Grove IoT Starter Kits Powered by AWS](/Grove_IoT_Starter_Kits_Powered_by_AWS "Grove IoT Starter Kits Powered by AWS") , [Seeeduino Cloud](/Seeeduino_Cloud "Seeeduino Cloud")*

**[Seeeduino Cloud](/Seeeduino_Cloud "Seeeduino Cloud")** is a microcontroller board based on Dragino WiFi IoT module [HE](http://www.dragino.com/products/linux-module/item/87-he.html) and ATmega32u4. **HE** is a high performance, low-cost 150M, 2.4G WiFi module which with an Open Source OpenWrt system inside. Seeeduino Cloud is also an [Arduino Yun](https://www.arduino.cc/en/Main/ArduinoBoardYun) compatible board. This kit includes most frequently used sensors and actuators to turn your ideas into tangible applications with AWS Cloud computing.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.amazon.com/dp/B01669BB60)

Features
--------

-   Out-of-the-box, plug and play, no breadboard or soldering work required.
-   Fully compliant with AWS's services and AWS's practices.
-   Step-by-step tutorials for developers and makers for quicker prototyping.

Included in the Box
-------------------

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Aws_kit_seeeduino_cloud.JPG)

| Board/Part                                                                                                                                            | Qty | Documentation                                                                 |
|-------------------------------------------------------------------------------------------------------------------------------------------------------|-----|-------------------------------------------------------------------------------|
| [Seeeduino Cloud development board](http://www.seeedstudio.com/depot/Seeeduino-Cloud-Arduino-Yun-compatible-openWRT-controller-p-2123.html?cPath=6_7) | 1   | [Read Here](/Seeeduino_Cloud "Seeeduino Cloud")                               |
| [Base Shield](http://www.seeedstudio.com/depot/Base-Shield-V2-p-1378.html?cPath=98_16)                                                                | 1   | [Read Here](/Base_shield_v2 "Base shield v2")                                 |
| [Grove - LCD RGB Backlight](http://www.seeedstudio.com/depot/Grove-LCD-RGB-Backlight-p-1643.html?cPath=34_36)                                         | 1   | [Read Here](/Grove-LCD_RGB_Backlight "Grove - LCD RGB Backlight")             |
| [Grove - Relay](http://www.seeedstudio.com/depot/Grove-Relay-p-769.html?cPath=39_42)                                                                  | 1   | [Read Here](/Grove-Relay "Grove - Relay")                                     |
| [Grove - Buzzer](http://www.seeedstudio.com/depot/Grove-Buzzer-p-768.html?cPath=38)                                                                   | 1   | [Read Here](/Grove-Buzzer "Grove - Buzzer")                                   |
| [Grove - Sound Sensor](http://www.seeedstudio.com/depot/Grove-Sound-Sensor-p-752.html?cPath=25_128)                                                   | 1   | [Read Here](/Grove-Sound_Sensor "Grove - Sound Sensor")                       |
| [Grove - Touch Sensor](http://www.seeedstudio.com/depot/Grove-Touch-Sensor-p-747.html?cPath=85_94)                                                    | 1   | [Read Here](/Grove-Touch_Sensor "Grove - Touch Sensor")                       |
| [Grove - Rotary Angle Sensor](http://www.seeedstudio.com/depot/Grove-Rotary-Angle-Sensor-p-770.html?cPath=85_52)                                      | 1   | [Read Here](/Grove-Rotary_Angle_Sensor "Grove - Rotary Angle Sensor")         |
| [Grove - Temperature Sensor](http://www.seeedstudio.com/depot/Grove-Temperature-Sensor-p-774.html?cPath=25_125)                                       | 1   | [Read Here](/Grove-Temperature_Sensor_V1.2 "Grove - Temperature Sensor V1.2") |
| [Grove - LED](http://www.seeedstudio.com/depot/Grove-LED-p-767.html)                                                                                  | 1   | [Read Here](/Grove-LED "Grove - LED")                                         |
| [Grove - Light Sensor](http://www.seeedstudio.com/depot/Grove-Light-Sensor-p-746.html?cPath=25_27)                                                    | 1   | [Read Here](/Grove-Light_Sensor "Grove - Light Sensor")                       |
| [Grove – Button](http://www.seeedstudio.com/depot/Grove-Button-p-766.html?cPath=85_50)                                                                | 1   | [Read Here](/Grove-Button "Grove - Button")                                   |
| DIP LED Blue-Blue                                                                                                                                     | 1   |                                                                               |
| DIP LED Green-Green                                                                                                                                   | 1   |                                                                               |
| DIP LED Red-Red                                                                                                                                       | 1   |                                                                               |
| Mini Servo                                                                                                                                            | 1   |                                                                               |
| Micro USB Cable - 48cm                                                                                                                                | 1   |                                                                               |

Configure Your AWS IoT Service
------------------------------

In this section, we will show how to:

1. Create an [AWS Account](http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/AMS5.0CreatingAnAWSAccount.html).

2. Go to [AWS IoT](http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/AMS5.0CreatingAnAWSAccount.html) and open the AWS IoT Dashboard.

Sign in with your AWS Account. Click the **Services** on the top-left corner, and then click on AWS IoT, as shown at below image.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_configure_AWS.png)

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_configure_AWS_click_service.png)

Click on **Get Started**.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_configure_AWS_click_get_started.png)

Then, we can create something now. Click on **Create a Resource** and then **Create a thing**.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_create_a_resource.png)

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_create_a_thing.png)

Enter a name, whatever you like, here we name it *temperature*.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_name_a_thing.png)

Click Create to complete it and then click **View thing** to get information of the thing you create.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_view_a_thing.png)

Click on **Connect a device**.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_connect_a_thing.png)

Choose **Arduino Yun** and Click on **Generate certificate and policy**.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_select_a_library.png)

It will show three download links which are correspond to different key files or certificate. Download these file, we need them later. And click on Confirm & start connecting.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_configure_AWS_download_keys_and_cofirm.png)

Then we should download the AWS IoT Arduino Yun SDK. Copy and save the sample code based on your behalf, we will need it later. And then click on Return to Thing Detail.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_configure_AWS_header_files.png)

Set up your Seeeduino Cloud (Arduino Yun)
-----------------------------------------

### Getting started with Seeeduino Cloud (Arduino Yun)

If this is your first time to use Seeeduino Cloud or Arduino Yun, you can click [here](/Seeeduino_Cloud) to get started. Before proceeding to the following steps, please make sure that you have **expect** installed on your computer and correctly installed the [Arduino IDE](https://www.arduino.cc/en/Main/OldSoftwareReleases).

### Installation on Mac OS/Linux

Before proceeding to the following steps, please make sure that you have **expect** installed on your computer and correctly installed the Arduino IDE.

#### To install expect

For Ubuntu, simply run the following command. sudo apt-get install expect For Mac OS X, **expect** is installed as default.

#### To install Arduino IDE

For Arduino IDE installation on Linux, please visit here (<http://playground.arduino.cc/Linux/All>).

#### Set up development board

1.Set up the Arduino Yún board and connect it to WiFi. Obtain its IP address and password. If you don’t know how to do it you can follow this [link](/Seeeduino_Cloud#Getting_Started).

2.Make sure your computer is connected to the same network (local IP address range).

3.Download the AWS IoT CA file from [here](https://www.symantec.com/content/en/us/enterprise/verisign/roots/VeriSign-Class%203-Public-Primary-Certification-Authority-G5.pem). And save it as *root-CA.crt*.

4.Put your AWS IoT CA file, private key and certificate into AWS-IoT-Arduino-Yun-SDK/AWS-IoT-Python-Runtime/certs.

5.Open a terminal, cd to **AWS-IoT-Arduino-Yun-SDK**. Do *chmod 755 AWSIoTArduinoYunInstallAll.sh* and execute it as:

```
./AWSIoTArduinoYunInstallAll.sh <Board IP> <UserName> <Board Password>.
```

By default for Seeeduino Cloud, your username will be root and your password will be seeeduino. Arduino Yún Board, your username will be root and your password will be Arduino.

For step 5, it can take 15-20 minutes for the device to download and install the required packages (distribute, python-OpenSSL, pip, paho-MQTT).

<div class="admonition note">
<p class="admonition-title">Note</p>
Do not close the terminal before the script finishes, otherwise you have to start over with step 5. Make sure you are in your local terminal before repeating step 5.
</div>

6.Copy and paste **AWS-IoT-Arduino-Yun-SDK/AWS-IoT-Arduino-Yun-Library** folder into Arduino libraries that was installed with your Arduino SDK installation. For Mac OS default, it should be under **Documents/Arduino/libraries**.

7.Restart the Arduino IDE if it was running during the installation. You should be able to see the AWS IoT examples in the Examples folder in your IDE.

There are the other two scripts: **AWSIoTArduinoYunScp.sh** and **AWSIoTArduinoYunSetupEnvironment.sh**, which are utilized in **AWSIoTArduinoYunInstallAll.sh**. You can always use **AWSIoTArduinoYunScp.sh** to upload your new credentials to your board. When you are in the directory **AWS-IoT-Arduino-Yun-SDK/**, the command should be something like this:

```
./AWSIoTArduinoYunScp.sh <Board IP> <UserName> <Board Password> <File> <Destination>
```

### Installation on Windows

Before proceeding to the following steps, please make sure that you have Putty and WinSCP installed on your PC. If you prefer to use other tools for SSH-ing into your Arduino Yún board and transferring files, you will have to adjust the steps below according to your tools. Putty can be downloaded from [here](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html). WinSCP can be downloaded from [here](http://winscp.net/eng/download.php). Set up the board.

1.Setup the Arduino Yún Cloud board and connect it to WiFi. Obtain its IP address and password. If you don't know how to do it, please follow this [link](/Seeeduino_Cloud#Getting_Started).

2.Make sure your PC is connected to the same network (local IP address range).

3.Download the AWS IoT CA file from [here](https://www.symantec.com/content/en/us/enterprise/verisign/roots/VeriSign-Class%203-Public-Primary-Certification-Authority-G5.pem). And save it as root-CA.crt

4.Put your AWS IoT CA file that you saved before, private key and certificate into folder **AWS-IoT-Arduino-Yun-SDK/AWS-IoT-Python-Runtime/certs**.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_set_up_arduino_yun_on_windows_copy_certs.png)

5.Start WinSCP and upload AWS-IoT-Python-Runtime/ folder to /root on the board.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_set_up_arduino_yun_on_windows_copy_run_time_file.png)

6.Use Putty to ssh into OpenWRT on your board and execute the following commands to install the necessary libraries:

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_set_up_arduino_yun_on_windows_login_dragino.png)

It can take 15-20 minutes for the device to download and install the required packages.

7.Copy and paste AWS-IoT-Arduino-Yun-SDK/AWS-IoT-Arduino-Yun-Library folder into Arduino libraries that was installed with your Arduino SDK installation. For Windows default, it should be under **Documents/Arduino/libraries**.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_set_up_arduino_yun_on_windows_copy_AWS_library_file_to_arduino_library.png)

8.Restart the Arduino IDE if it was running during the installation. You should be able to see the AWS IoT examples in the Examples folder in your IDE.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_set_up_arduino_yun_on_windows_load_example.png)

### Connect Grove Module

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_set_up_arduino_yun_on_windows_hardware_connection.png)

Run examples
------------

### Download the example project

1.Please download the example project from [here](https://github.com/Lee-Kevin/10.GroveWithAWSIot/) first.

2.Decompress the downloaded zip files to your computer and remove **-master** in decompressed file name.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_open_example_sketch.png)

### Modify header file

1.Open file **aws_iot_config.h**, and replace the content in red box as picture bellows by the sample code based on your account that you have already saved before.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_run_example_replace_header_file.png)

2 .Double click on **GroveWithAWSIot.ino**, replace following marked code with saved header file minutes ago and then click upload.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_run_example_select_serial_port.png)

3 .When you see the below info. it means you have already download the code to your Seeeduino Cloud successfully.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_run_example_upload_complete.png)

### View Result

1 .Open the serial monitor, you can see the information as below.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_run_example_view_result_in_serial_monitor.png)

2 .Then open AWS IoT website, sign in to your account. And click the thing you created minutes ago.

Click the **Update shadow** button. Now you can see the temperature was upload to the website.

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS/master/img/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS_run_example_reopen_thing_and_update_shadow.png)

Resources
---------

-   [AWS IoT Documentation](http://aws.amazon.com/documentation/iot/)
-   [Seeeduino Cloud wiki page](/Seeeduino_Cloud)
-   [AWS IoT Arduino Yún SDK](https://github.com/aws/aws-iot-device-sdk-arduino-yun#yield)


-----------------------------------------------------------------------------------

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Seeeduino_Cloud_and_Grove_IoT_Starter_Kit_Powered_by_AWS -->
