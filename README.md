# Blinds
Stepper drivers TMC2209
https://amzn.to/3oHofrM

Stepper Motors 28byj 48
https://amzn.to/3AA7ZLL

Howto control stepper motors (not my work)
https://github.com/arendst/Tasmota/discussions/11731

I have added my backup configuration file. you can upload it and change your mqtt and wifi informaiton . 

•	Run commands in the console to run the "Shutter" mode (you must first configure the GPIO!):
SetOption80 1 // Enable shutters support.
ShutterMode 4 // Enable "Shutter mode 4".
ShutterRelay1 1 // for relay Relay1 and Relay2.
ShutterRelay2 3 // for relay Relay3 and Relay4.
Restart 1 // Restart Tasmota.
•	Run commands in the console to configure the motor operation (you must first configure the GPIO!):
ShutterFrequency 2000 // This is a global variable for all steppers (default = 1000ppm).
ShutterMotorDelay1 1.5 // Shutter#1 acceleration/deceleration speed for stepper motor(default = 0 seconds).
ShutterOpenDuration1 15 // Shutter#1 opening time = 15 seconds (default = 10 seconds).
ShutterCloseDuration1 15 // Shutter#1 closing time = 15 seconds (default = 10 seconds).
ShutterMotorDelay2 1.5 // Shutter#2 acceleration/deceleration speed for stepper motor(default = 0 seconds).
ShutterOpenDuration2 15 // Shutter#2 opening time = 15 seconds (default = 10 seconds).
ShutterCloseDuration2 15 // Shutter#2 closing time = 15 seconds (default = 10 seconds).
Restart 1 // Restart Tasmota.

