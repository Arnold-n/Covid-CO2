# covid-CO2 CO2 sensor
![Sensor image with battery](Pictures/sensor1.jpg)
![Sensor image without battery](Pictures/sensor2.jpg)

This project explains how to build a small, light and affordable DIY CO2 sensor useful to measure CO2 levels in indoor locations. CO2 can be used as a proxy to estimate the COVID-19 infection risk by aerosols, and thus to control ventilation (opening windows depending on CO2 levels, balancing cold and risk). Being portable it can be used to verify ventilation status in supermarkets or schools.

## Functionality 

The CO2 sensor has:
- an OLED display for CO2 measurement, and a graph for the past hour (default graph range is 400-1000ppm, dashed indicator line at 600ppm)
- optional LED with blinking pattern depending on CO2 level (thresholds at 600, 800, and 1000ppm)
- optional Li-ion battery with on/off switch and battery voltage indicator

It measures ca 20x35x55mm without battery, or ca 20x35x84mm with battery.

It is powered over micro-USB.

## Known problems

The LED blinks (also <600ppm) if the device is not connected to WiFi. A solution (new firmware images) will be posted soon.

## Project overview

There is a detailed illustrated building guide, and pre-built firmware images and 3D print files are provided. The only necessary software effort is to flash an initial Tasmota image to an ESP8266 board. There are different firmware versions depending on the CO2 sensor:
- Winsen MH-Z19B sensor with automatic baseline calibration off
- Winsen MH-Z19B sensor with automatic baseline calibration on
- SenseAir S8 sensor
- Sensirion SCD-30 sensor

There are different STL files to print a 3D-case (one bottom and one top file per case) for
- Winsen MH-Z19B version without battery
- Winsen MH-Z19B version with battery
- SenseAir S8 LP version without battery
- SenseAir S8 LP version with battery
- Sensirion SCD-30 version without battery (will be uploaded later)
- Sensirion SCD-30 version with battery (will be uploaded later)
