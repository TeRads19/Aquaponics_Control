# Aquaponics_Control
Arduino Code for Control Node on Aquaponics Projects.

## DEVICE SPECIFICATION

* FireBeetle ESP32 IoT Microcontroller
* DFRobot pH sensor pro V2 kit
* DFRobot analog Dissolved Oxygen sensor kit
* DFRobot TDS sensor kit
* Dallas Semiconductor DS18B20 Temperature sensor
* Arduino Uno R3
* RobotDyn dual channel AC Dimmer & Zero-Crossing module
* Nextion NX4832K035 Resistif TFT touchscreen.


## Control System Schematics
![Example Image](https://drive.google.com/uc?id=1mMVa8zDyjzyA-RP0FeLBaGFyblFXNmOj)

## FIS Control


### Fuzzyfication
On fuzzyfication step, the input from each parameter (pH, TDS, DO and Temperature) converted into fuzzy value based on the respective membership function. Here is the image showing the membership function of each input parameter

![pH Membership Function]()
![DO Membership Function]()
![TDS Membership Function]()
![Temperature Membership Function]()


### Inference
On this project i use 160 Fuzzy Rule-Base to get the implication result for output value of water pump and aerator

### De-Fuzzification

## IMPORTANT NOTES





