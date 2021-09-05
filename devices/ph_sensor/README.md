
# PH Sensor

An ESP32 connected to a PH Sensor and logging data into Home Assistant using ESP Home

[TOC]

# Parts List

- ESP32
- PH Sensor and calibration fluid
- 5V Regulated power supply
- Analog to Digital converter
- Pin Headers
- Perf board
- 22AWG wire
- pc mount barrel plug power connector


## ESP32
 The layout detailed is for the ESP32 30 Pin board

[![](https://circuits4you.com/wp-content/uploads/2018/12/ESP32-Pinout.jpg)](https://circuits4you.com/wp-content/uploads/2018/12/ESP32-Pinout.jpg)


## PH Sensor
I am using the DF Robot PH Sensor https://www.dfrobot.com/product-1782.html , cheaper alternatives are available on aliexpress but in testing have not been as reliable or long lasting


## Power Supply
A seperate 5V DC power regulated power supply was required as when using the ESP32s 5V USB power supply the PH probe worked fine during development but with PH probe inserted into the pool pipe the signal fluctuated widely.

The ESP32 also performed fine when connected to a 9V DC regulated power supply

Using a seperate power supply the signall does tend to still vary when pumps are running but in the range of 0.1 PH

## Analog to Digital converted
ADS1115, The ADS1115 analog to digital converter is required as the inbuilt A2Cis not accurate enough.

## Pin Headers
Male and Female pin headers are required as part of making the board

## Perf board
A 5cm square 19x19 perf board is used for the layout, anything around that size would be fine

## 22AWG wire
For connecting parts.

## Power connector
A pc mount barrel plug power connector makes it easy to connect and disconnect the power supply as required.

## Board Layout
<img src="../../devices/ph_sensor/ph%20sensor.png">


