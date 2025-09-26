 smart Home Environment Monitor

A compact, Arduino-based system that monitors indoor temperature, light, and sound levels using analog and digital sensors. Designed for modularity, real-time feedback, and easy simulation in Tinkercad, this project is ideal for DIY home automation and environmental awareness

 Features

Temperature Monitoring(via potentiometer)
Ambient Light Detection (via photoresistor)
Sound Detection(via push button and simulated microphone)
Alert System with LED and buzzer
LCD Displayfor real-time feedback
Tinkercad Simulation with analog substitutes



 Components Used

Inputs
 Component        Pin    Purpose                          

 Potentiometer   A0     Simulates temperature sensor     
 Photoresistor   A1     Measures ambient light           
 Potentiometer   A2     Simulates microphone/sound level 
 Push Button     D11    Detects sound events (digital)   

Outputs
 Component        Pin   Purpose    
 
 LED            D13      Visual alert                     
Buzzer          D12     Audible alert                    
LCD (I2C, 0x27) SDA/SCL  Displays sensor data and alerts 

Tinkercad Simulation Notes

Tinkercad does not support microphone sensors, so this project uses a second potentiometer on A2 to simulate analog sound input.

Adjusting the potentiometer mimics changing sound levels.
The push button provides binary sound detection.
This setup allows full testing of alert logic and display behavior.

When deploying on real hardware, replace the A2 potentiometer with a microphone module like KY-038**, MAX4466, or LM393.

Alert Conditions

The system activates the buzzer and LED when:
 Temperature exceeds 35°C
 Light level exceeds 80%
 Sound button is pressed
 Simulated microphone level exceeds 70%

Serial Output Example

Temp: 28°C  Light: 45%  Sound Btn: NO  Mic Level: 62

