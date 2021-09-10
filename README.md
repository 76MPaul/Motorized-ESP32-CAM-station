# Motorized-ESP32-CAM-station

## Introduction : 

This project is an evolution of other motorized ESP32cam projects.
WIth this station, everything is nearly hidden inside the tower. It includes the room for a DHT22 sensor to complete the station. 

I developed the arduino code with MQTT integration to get/control the whole thing with Home Assistant.

## Pré-requis :
*   [Print the 3D model]()
*   2 SG90 servo motors
*   1 ESP32 cam
*   1 micro USB port
*   1 DHT22 sensor
*   jump wires

## Configuration : 
Edit the WIFI inside the home_wifi_multi.h file
Edit the MQTT credentials on line 418 // ------------ MQTT ------------
Edit then the MQTT topics to match your needs.

Edit the servo pinout on line 383 // ------------ SERVOS ------------
Edit the DHT pinout on line 403 // ------------ DHT ------------
Upload the code on your ESP.

Home assistant [Tutorial and informations on my website](https://www.paulmagnier.fr/station-motorisee-pour-esp32cam/)

## Usage :
Read value from the MQTT Topic
Send integer values from 0 to 180 on the two slider topics.
