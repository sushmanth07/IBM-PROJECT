# IBM-PROJECT


# Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan
SMART WATER MANAGEMENT

1) Directly you can simulate this model by using this link : https://wokwi.com/projects/380553351208403969 
And should follow the steps provided in 3) THINGSPEAK and 4) REAL-TIME VIEWING PLATFORM which is below in this readme file


Or Otherwise to build this :

2) WOKWI:
First we should design the model which is in the image below:

![Screenshot from 2023-11-05 23-58-04](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/f7d64529-38a9-4432-8948-c39ce50ebd18)

First Components Needed:
a) ESP32
b) Ultrasonic Sensor
c Potentiometer
d) VCC
e) GND

![Screenshot from 2023-11-05 11-36-27](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/a04024ea-f9fb-4706-be64-a7463c044e54)


Connections:

Ultrasonic Sensor Connections:
i) Connect VCC of Ultrasonic Sensor to VCC which we added.
ii) Connect GNG of Ultrasonic Sensor to GND which we added.
iii) Connect TRIG of Ultrasonic Sensor to esp:26 in ESP32.
iv) Connect ECHO of Ultrasonic Sensor to esp:25 in ESP32.

![Screenshot from 2023-11-05 15-48-57](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/ab763edd-c4fb-40a7-a26d-d763ee5d8cb4)

Potentiometer Connections:
i) Connect VCC of Potentiometer to esp:3V3 of ESP32.
ii) Connect GND of Potentiometer to esp:GND.2 of ESP32.
iii) Connect SIG of Potentiometer to esp:3 of ESP32.

![Screenshot from 2023-11-05 15-49-31](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/9a7aa077-d736-4a49-a8fa-b476734099fc)




Then we should use the sketch.ino file.
The diagram.json will be updated as we design the model in first step.
Then we should install needed libraries which is in libraries.txt.
We should change the CHANNEL ID and API_KEY of ThingSpeak in this code to your ThingSpeak channel's ID and API_KEY.

![Screenshot from 2023-11-06 01-55-48](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/a1695cdb-ccca-493e-9b48-aae03d04e3e4)


Then we can run the program .
And we can get output of the model.

![Screenshot from 2023-11-06 01-56-28](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/ada037bb-aec9-4206-bc27-38ccdf87f727)


Here we get the water level output and ph value which tels whether the water is contaminated or not.

3) THINGSPEAK:
Then we want to open an account in ThingSpeak and should create a New Channel.
And Should create two fields named water level in CM and pH value.

![Screenshot from 2023-11-05 16-24-22](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/004a480a-b077-442f-b220-20cc66a538e7)


We will connect the wokwi model to this ThingSpeak by using the CHANNEL ID and API_KEY of your ThingSpeak channel.
Then we want to run the Wokwi model and we will get the output data in ThingSpeak as Values and Graphs.

![Screenshot from 2023-11-05 16-32-01](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/30386aa0-2395-40a7-8ee7-ae9ba21b6437)


4) REAL-TIME VIEWING PLATFORM:
First change the CHANNEL ID and API_KEY to your ThingSpeak channel in the index.html file ,and also use the background image which is named as Waterimage.jpg and then run the file.

![Screenshot from 2023-11-06 01-58-41](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/e5859abb-7b74-40b9-9d86-e2280bcf709b)


Then we will see two buttons which is Water Consumption Data and Contamination Level Data.

![Screenshot from 2023-11-05 16-33-02](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/29806047-c1ef-47f3-b20f-3bf30d2f3681)


When we click the Water Consumption Data button then we will get the value in centimetres.

![Screenshot from 2023-11-05 16-33-13](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/a5f387c1-9573-4c08-933b-0ff481ed6ce1)




When we click the Consumption Level Data button then we will get the output of pH value and it will tel whether the water is contaminated or not.

![Screenshot from 2023-11-05 16-33-21](https://github.com/ROHITKANNAGITHUB/Rohit-Kanna-.S-Internet-Of-Things-Naan-Mudhalvan/assets/98509320/848011f1-17a0-4bea-b028-b4c1b0da795f)





