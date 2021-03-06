---
layout: documentation
title: HS1HT-Z  - ZWave
---

{% include base.html %}

# HS1HT-Z Temperature/Humidity Sensor
This describes the Z-Wave device *HS1HT-Z *, manufactured by *[Heiman Technology Co. Ltd](http://www.heimantech.com/)* with the thing type UID of ```heiman_hs1htz_00_000```.

The device is in the category of Sensor, defining Device used to measure something.

# Overview

Smart Temperature and Humidity Sensor is designed to detect the temperature and humidity in house, and reports the abnormal conditions to users' mobile phone, Users could also check the real-time temperature and humidity via mobile phone, The sensor adopts Z-Wave wireless communication protocol with high sensitivity.

See:   
https://products.z-wavealliance.org/products/2321  
and  
http://www.heimantech.com/product/80.html

## Inclusion Information

Click \[Add\] icon in Z-Wave Controller.  
\- Press the Net\_Button 3 times within 1.5s, Green LED is Blinking 3 times within 1 second.  
\- If Inclusion Process is successful, Green LED will turn off.

## Exclusion Information

Click \[Remove\] icon in Z-Wave Controller.  
\- Press the Net\_Button 3 times within 1.5s   
\- If Exclusion Process is successful, Green LED is Blinking 6 times, then turn off

## Channels

The following table summarises the channels available for the HS1HT-Z 

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Sensor (temperature) | sensor_temperature | Temperature | Number | 
| Sensor (relative humidity) | sensor_relhumidity | Humidity | Number | 

### Sensor (temperature)

Indicates the current temperature

The ```sensor_temperature``` channel supports the ```Number``` item and is in the ```Temperature``` category. This is a read only channel so will only be updated following state changes from the device.

### Sensor (relative humidity)

Indicates the current relative humidity

The ```sensor_relhumidity``` channel supports the ```Number``` item and is in the ```Humidity``` category. This is a read only channel so will only be updated following state changes from the device.



## Device Configuration

The device has no configuration parameters configured.

## Association Groups

Association groups allow the device to send unsolicited reports to the controller, or other devices in the network. Using association groups can allow you to eliminate polling, providing instant feedback of a device state change without unnecessary network traffic.

The HS1HT-Z  supports 3 association groups.

### Group 1: Lifeline

Association group 1: Lifeline association group Maximum supported node is 1. Include command classes: Battery report, multilevel sensor report, and Device Reset Locally.
This group supports 1 nodes.

### Group 2: Multilevel sensor temperature

Association group 2: Root Device group(multilevel sensor temperature) Maximum supported nodes are 5. 1- multilevel Sensor reports status of the temperature via Lifeline. 2-When the sensor detects status of the temperature, the device will be triggered.
This group supports 5 nodes.

### Group 3: Multilevel sensor humidity

Association group 3: Root Device group(multilevel sensor humidity) Maximum supported nodes are 5. 1-multilevel Sensor reports status of the humidity via Lifeline. 2-When the sensor detects status of the humidity , the device will be triggered.
This group supports 5 nodes.

## Technical Information

### Endpoints

#### Endpoint 0

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_NO_OPERATION_V1| |
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SENSOR_MULTILEVEL_V10| Linked to BASIC|
| COMMAND_CLASS_ASSOCIATION_GRP_INFO_V1| |
| COMMAND_CLASS_DEVICE_RESET_LOCALLY_V1| |
| COMMAND_CLASS_ZWAVEPLUS_INFO_V2| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V2| |
| COMMAND_CLASS_POWERLEVEL_V1| |
| COMMAND_CLASS_BATTERY_V1| |
| COMMAND_CLASS_WAKE_UP_V2| |
| COMMAND_CLASS_ASSOCIATION_V2| |
| COMMAND_CLASS_VERSION_V2| |

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/709).
