# Obstacle-Avoiding-Robot

#  Obstacle Avoiding Robot using ESP32
##  Project Overview
This project demonstrates a simple **Obstacle Avoiding Robot** using an ESP32, an ultrasonic sensor, and a motor driver module.
The robot measures the distance in front of it using an ultrasonic sensor.  
If the path is clear, the robot moves forward.  
If an obstacle is detected within a certain distance, the robot stops to avoid collision.

## Features
- Detects obstacles using an ultrasonic sensor
- Automatically moves forward when the path is clear
- Stops when an object is detected
- Displays distance in Serial Monitor
- Simple autonomous robot behavior
- 
##  Components Used
- ESP32
- Ultrasonic Sensor (HC-SR04)
- Motor Driver (L298N / L293D)
- 2 DC Motors
- Robot Chassis
- Battery Pack
- Jumper Wires

## Pin Configuration

 Component---->ESP32 Pin 
 Ultrasonic TRIG ---->GPIO 5 
 Ultrasonic ECHO ----> GPIO 18 
 Motor IN1 ----> GPIO 26 
 Motor IN2 ----> GPIO 27
 Motor IN3 ---->GPIO 32 
 Motor IN4 ----> GPIO 33 


## Working Principle

1. The ultrasonic sensor sends a sound wave from the **TRIG pin**.
2. The sound wave hits an object and reflects back to the **ECHO pin**.
3. ESP32 calculates the distance using the time taken for the echo.
Distance formula used:
Distance = (Duration × 0.034) / 2

4. If the distance is **greater than 30 cm**  
   → The robot **moves forward**.

5. If the distance is **less than or equal to 30 cm**  
   → The robot **stops** to avoid collision.

##  How to Run the Project

1. Connect all components according to the pin configuration.
2. Open Arduino IDE.
3. Select the **ESP32 board**.
4. Upload the code to ESP32.
5. Power the robot using a battery.
6. The robot will move forward and stop when it detects an obstacle.

##  Concepts Used

- Ultrasonic sensor distance measurement
- Motor control using GPIO pins
- Embedded system programming
- Conditional logic
- - Basic robotics automation

##  Learning Outcomes
- Understanding ultrasonic sensor working
- Interfacing sensors with ESP32
- Controlling motors using microcontrollers
- Implementing basic autonomous robot behavior
- Designing simple robotics projects

##  Possible Improvements

- Add left/right turning for better obstacle avoidance
- Use multiple ultrasonic sensors
- Add Bluetooth control
- Add line following + obstacle avoidance hybrid robot
- Use PID control for smoother movement
  
##  Author
Harsha G  
Learning **Python | Embedded Systems | IoT | Robotics**
