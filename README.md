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
To build the fis algorithm, i'm using matlab to write the code and choose the mamdani fuzzy method. The weight of all input and output is set equal (1). And for converting into arduino code file (.ino) im using online tools [fis to ino converter](http://www.makeproto.com/projects/fuzzy/matlab_arduino_fist/index.php)

on fuzzy inference system, there are 3 major step for system to be able to determine the respective output value based on a certain scenario.

### Fuzzyfication
On fuzzyfication step, the input from each parameter (pH, TDS, DO and Temperature) converted into fuzzy value based on the respective membership function. Here is the image showing the membership function of each input parameter.

* ![pH Membership Function]()
* ![DO Membership Function]()
* ![TDS Membership Function]()
* ![Temperature Membership Function]()

All membership function set based on literature that i used on my research publication. You could find the publication in [here]().

### Inference
On this project, i use 160 Fuzzy Rule-Base to get the implication result for output value of water pump and aerator.

### De-Fuzzification
After the implication value of water pump and aerator done calculated, the fuzzy value will be converted back into crisp value using Centroid method.

Centroid method is .......

## Output Control Using AC Dimmer & Zero-Crossing Module
This project using AC (Alternating Current) water pump and aerator. You are welcome to use any DC sourced water pump and aerator for your own project, if so you wouldn't needed the AC Dimmer PWM function on actuator control source code. You can use a direct PWM value and make your own function to control your output based on the behavior of water pump and aerator that you use.

### Brief explanation on how AC Dimmer works



## IMPORTANT NOTES





