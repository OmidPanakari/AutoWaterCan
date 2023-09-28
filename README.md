# AutoWaterCan
Automatic Irrigation System
# Description
AutoWaterCan is a system that is designed to automatically irrigate your plants. For this purpose, it measures humidity and temperature of the plant's environment constantly and based on that, it changes the amount of water which is used for irrigating the plant.
This system consists of three parts: Sensor, Actuato and Central part. For implementing each of these parts, an Arduino uno microcontroller board was used and these boards communicate with each other using bluetooth module
[HC-05](https://components101.com/sites/default/files/component_datasheet/HC-05%20Datasheet.pdf). This design is done using Promtheus simulation tool.
## Sensor
In order to measure values of humidity and temperature, [SHT-25](https://www.mouser.com/datasheet/2/682/Sensirion_Datasheet_Humidity_Sensor_SHT25-3051651.pdf) was used. After each update from the sensor, the board
calculates the desired values based on formulas provided in the datasheet and then sends these values to the central part.
![image](https://github.com/OmidPanakari/AutoWaterCan/assets/78135553/3a4f6295-fc19-464d-b66e-f4da0a959284)

## Central
After receiving values from the sensor part, this part decides what amount of water is needed for irrigation and then regarding to it, the speed of DC motor, that is used for sending water to plant, is calculated and
sent to actuator part.
![image](https://github.com/OmidPanakari/AutoWaterCan/assets/78135553/cf64406c-8c26-4984-a6b0-fc0d168849fa)

## Actuator
Finally, this part uses DC motor for controlling amount of water which is sent to the plant.
![image](https://github.com/OmidPanakari/AutoWaterCan/assets/78135553/b7497c8a-6687-414b-a20d-59a7cc470953)

In the image below, all three parts can be seen working together.
![image](https://github.com/OmidPanakari/AutoWaterCan/assets/78135553/e6ce5560-a4e1-43ff-8016-c749c8dc04da)
