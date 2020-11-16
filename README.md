**Remote Physiotherapy System made using LoRa &amp; ML**


**Short Description -**


A smart device built for remote physiotherapy services for old-age people , which sends up
exercising data upto any doctor’s clinic using LoRa protocol. The device is extremely energy
efficient and can be used from any part of the world and there is no need for any wireless
networks needed for using the device. The device uses LoRa and is powered by Edge
Impulse’s efficient and accurate ML models. The device consists of two parts - a small LoRa
Node and a multi-channel gateway which will remain stationary and will be able to receive
the data.

**Complete Explanation -**

Okay so the thing is that the WisBlock board has the ability to communicate with some pretty excellent sensors directly....here we will be using Accelerometer sensor attached to the WisBlock starter board kit and then I will send up the sensor data to the Edge Impulse CLI using serial communication and then I will make a Tensorflow model which will run on the board itself (no need of connecting to any cloud or whatever).
The main idea is that many patients who are in their 70's or older experience pain on their muscles and bones and need some physiotherapy exercises to be able to move their muscles and bones (some biology stuff) and then it will help the doctors to remotely communicate with the patients and know when and how well they are doing their regular exercises and stuff remotely using Edge Impulse and sending data using LoraWAN.


**Hardwares required -**

● WisBlock Base Board

● WisBlock Core Board

● WisBlock 3-axis accelerometer Sensor

● RAK Discover 2 Gateway kit

**Softwares required -**

● Edge Impulse studio (for training the model and doing a live classification)

● balenaCloud and balenaOS (for enabling the LoRa gateway to communicate to TTN using the latest LoRa BasicStation protocol) 

● The Things Network (sending data to TTN server and sharing the data feed to the
doctor)

● Arduino IDE (putting the C++ code to the WisBlock board)

**Brief Circuit explanation -**

WisBlock Base Board + Core Board + Sensor ↠ TTN server ↠ Gateway ↠ back to
doctor’s mobile phone/device

**Objectives-**

*1) What need do you see in the community for the problem you are trying to solve?*

Senior Citizens or aged people usually face the Chronic disease of Arthritis which requires physiotherapy treatment.
Have a look at this article - https://www.thephysiocompany.com/blog/how-physiotherapy-can-help-older-people

*2) What medical knowledge do you have to be able to solve the problem in the right way?*

I got the actual project idea from my Dad who is a Physiotherapist. He said me about the instances that people in the old age experience and why there hasn't been any technologies developed for that. 

*3) Where will the device be used? In the clinic? In the patient’s home? What if the patient does not have access to LoRa coverage?*

The RAK Discovery 2 Gateway will be present on the doctor's clinic/lab and the WisBlock board (which will act like the node) will be present in the patients home. 
Even if the patient has no LoRa coverage in that are then we can make use of the Ultra Low power but highly efficient nRF52840 chipset present on board which can send and transfer data using BLE or we can even add an ESP32 module to it as WisBlock boards are expandable , which will enable us to communicate using highly powerful WiFi and BLE which can then send the ML data to the Ubidots server and it could forward the data to the doctor directly. 

*4) Why use WisBlock for this project?*

WisBlock are the latest released LoRa boards which are very developer friendly and can be easily expandable, the main fact is that it can communicate via most types of data transfer protocol such as LoRa , NB-IoT , WiFi and BLE. Also it uses a nRF52840 chipset on board which is self sufficient enough to take our ML model to run on that tiny little board. Moreover using WisBlock board is an excellent choice for this project. 

**Build Logs**
*Coming Soon! Stay Tuned!*

**Project Authors**

Arijit Das 

María Carlina Hernández

Diana Rodriguez

**Copyright & License**

This is an open-source project made possible with the great support from RAK Wireless & Edge Impulse team. 

This project currently occupies an Open-Source MIT License. 

© MIT
