# Smart-Irrigation-System-using-IoT

Most farmers having large portions of farming land find it very difficult to reach and track the moisture levels at each corner of their land from time to time. So there is a possibility of uneven water sprinkles. This result in the bad quality crops which further leads to financial losses. Hence in such scenario, Smart Irrigation Techniques using latest IoT technologies is extremely hepful and leads to ease of farming.

In this mini project, I have made an IoT based Smart Irrigation System using ESP8266 NodeMCU Module and DHT11 temperature and humidity sensor. It will not only automatically irrigate the water based on the moisture level in the soil but also send the data to ThingSpeak Server to keep track of the land condition. 

The System will consist of a water pump which will be used to sprinkle water on the land depending upon the land environmental condition such as moisture, temperature and humidity. 

                  Components Required for this IoT based Smart Irrigation System
                
The components needed for this mini project are as follows:

1> NodeMCU ESP8266

2> Soil Moisture Sensor Module

3> Water Pump Module

4> Relay Module

5> DHT11 temperature and humidity sensor

6> Connecting Wires

7> Breadboard


In this project, I have preferred NodeMCU over Arduino primarily due to its easy Wifi connectivity capabilities. This is because Node MCU board has ESP-8266 (WiFi Modules) chips on it which helps to connect the entire system to internet directly. I have also connected our system to the ThinkSpeak server, so as to be able to visualize the moisture, temperature and humidity data of our sample soil while the system operates.


# The Circuit Diagram of this project is shown as:

![proj3](https://user-images.githubusercontent.com/64331214/146637042-c2248dee-401b-488c-95e8-19002f483244.png)


# Working Procedure

Since different crops have different moisture requirements, here we consider a sample crop which will require a soil moisture of about 50-55%. Thus we program our NODEMCU accordingly.

1> As the system is powered, the soil moisture sensor module will sense the instantaneous moisture of the soil.

2> When the soil loses its moisture to less than 50%, then NodeMCU will cause the Motor pump to turn on automatically to sprinkle the water and it will continue to sprinkle the water until the moisture goes upto 55%. After that the motor pump will automatically be turned off. Thus the moisture level of the crop is being taken care of automatically.

3> The DHT11 sensor additionally records the temperature and humidity of the atmosphere continuously.

4> These sensor datas of temperature, moisture and humidity will be sent to the ThinkSpeak server at defined intervals of time, so that the conditions can be monitored from anywhere.
