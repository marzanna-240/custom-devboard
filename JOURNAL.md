---
title: "Custom Devboard"
github: "https://github.com/marzanna-240/custom-devboard"
description: "A custom devboard using the ESP32-S3-WROOM-2 Microcontroller."
created_at: "25/11/2026"
total_time: ""
---

## 26/11/2026: <Entry no.0>

First journal entry!
I based the idea of this project off of the Arduino Uno Q, since I really liked the look of the charlieplexed LED matrix that the board uses. 
A lot of the time spent here was doing research from the Arduino and ESP32 datasheets, since I'm still figuring out which components are needed.
So far I've got the USB receptacle, LDO regulator, LED matrix and decoupling capacitors set up. Next I'll be figuring out the boot and reset buttons for the microcontroller since I don't really know how it works for the ESP32 yet. 

<img width="2220" height="1555" alt="image" src="https://github.com/user-attachments/assets/075f84fd-080a-46b3-812d-a36d0c4e1917" />

**Total time spent: 2h**

## 27/11/2026: <Entry no.1>

Today I've finished laying down my schematic. Everything is set up and should be ready for the PCB.
I had to create new footprints for the ESP32 and CP2102 since the ones I was using before had incorrect pinouts, then I set up all the supporting components for the CP2102 by following the ESP32 hardware documents. I've also set up the boot, reset buttons and auto programming circuit for convenience. There are now 8 designated pins for the LED matrix, I'm not sure if there's a way to do it without sacrificing the pin's GPIO functionality, since now they can only be used for the LED matrix instead of anything else, but maybe that's for a future project. For the rest of the pins there are two male header pins, one is 12x1 and the other is 20x1, each has 2 GND pins and the 12x1 header has a 3.3v pin and a 5v pin. 

<img width="2495" height="1692" alt="image" src="https://github.com/user-attachments/assets/716b7dd8-f5f0-4ba9-baab-f38c0af7ec81" />

**Total time spent: 3h 39m**

