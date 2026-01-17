# TASK-2
Sensor Data Logging to SD Card using Arduino 

Project Overview :
     This project demonstrates sensor data acquisition and logging using Arduino.
     Environmental sensor values (temperature and light) are sampled at fixed intervals and stored as timestamped CSV entries on an SD card.
     This project was implemented as part of the Embedded Systems Internship at Alfido Tech.

Objectives :

Read sensor data periodically
Add accurate timestamps to each sample
Store data in CSV format on an SD card
Understand sampling rate and power considerations

Hardware Used :

Arduino (SPI supported)
SD Card Module
Temperature Sensor
Light Sensor (LDR)
RTC Module (DS1307 / DS3231)
Jumper Wires

Software & Libraries :

SD.h
SPI.h
RTClib (for RTC timestamping)

Working Principle :

Sensors are read at a fixed sampling interval.
RTC provides current date and time.
Each reading is stored as a new row in a CSV file:
Timestamp, Temperature, Light
Data is appended until required samples are collected.

Sampling Rate & Power Considerations :

Sampling interval is set using delay() / timer logic.
Lower sampling rates reduce:
Power consumption
SD card write cycles
SD card is accessed only during write operations to save power.

How to Run :

Connect sensors, RTC, and SD card module
Insert formatted SD card
Upload code to Arduino
Power the system
Remove SD card and open CSV file on PC

Output :

CSV file with 100+ timestamped sample
Each row contains sensor values with date and time

Skills Demonstrated :

Sensor interfacing
SD card data logging
SPI communication
RTC usage
Embedded system design considerations

Internship
Embedded Systems Internship – Alfido Tech

