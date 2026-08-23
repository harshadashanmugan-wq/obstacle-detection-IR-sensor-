IR Obstacle Detector
1. Project Overview

This project is a simple IR-based obstacle detection system that detects the presence of an object using an IR LED and photodiode.
The IR LED continuously emits infrared light. When an obstacle comes in front of the detector, the infrared light is reflected back toward the photodiode. The change in the photodiode signal is then used to activate a transistor switching circuit.
When an obstacle is detected, a buzzer and LED provide an alert.

Basic Concept

IR LED → Infrared Signal → Obstacle → Reflected IR → Photodiode → Transistor Switch → Buzzer + LED

2. Objective
To understand the working principle of infrared obstacle detection.
To interface an IR LED and photodiode.
To understand photodiode-based sensing.
To use transistors as switching stages.
To activate an LED and buzzer when an obstacle is detected.
To develop a simple and low-cost obstacle detection system.

3. Working Principle
The system consists of two main sections:

1. IR Transmitter

An IR LED is used as the transmitter.
The IR LED continuously emits infrared radiation toward the area in front of the detector.
When there is no obstacle, most of the emitted infrared radiation does not return to the receiver.

2. IR Receiver

A photodiode is used to detect the reflected infrared radiation.
When an object comes close to the detector, infrared light is reflected from the object and reaches the photodiode.
The resulting change in the photodiode signal is applied to the transistor circuit.

3. Transistor Switching

The circuit uses two BC547 transistors.
The transistor stages process the signal from the photodiode and act as switching/amplification stages.
When the detected signal reaches the required level, the transistor stages activate the output section.

4. Alert System

When an obstacle is detected:

🔴 LED turns ON
🔊 Buzzer produces an alert

This provides both visual and audible indication of an obstacle.

4.Components Used
IR LED
Photodiode
BC547 × 2
LED
Buzzer
180 Ω resistor
56 kΩ resistor
2.8 kΩ resistor
9 V battery/power supply
Connecting wires
Breadboard
🔋 Circuit

The circuit is powered using a 9 V supply.

Main Circuit Sections
                 9V Power Supply
                       │
          ┌────────────┴────────────┐
          ↓                         ↓
      IR LED                    Photodiode
     Transmitter                  Receiver
          │                         │
          │                    BC547 Stage 1
          │                         │
          │                    BC547 Stage 2
          │                         │
          │                    Output Stage
          │                         │
          └──────────────→ Buzzer + LED
5. Block Diagram
       POWER SUPPLY
             │
             ↓
       IR TRANSMITTER
             │
       Infrared Light
             ↓
          OBSTACLE
             │
      Reflected IR Light
             ↓
        IR RECEIVER
       (Photodiode)
             │
             ↓
     SEMICONDUCTOR SWITCH
       (BC547 Transistors)
             │
             ↓
       BUZZER + LED
🔍 Operation
No Obstacle
IR LED
  ↓
Infrared radiation
  ↓
No significant reflection
  ↓
Photodiode signal remains below switching condition
  ↓
Buzzer OFF
LED OFF
Obstacle Detected
IR LED
  ↓
Infrared radiation
  ↓
Obstacle
  ↓
Reflected infrared radiation
  ↓
Photodiode
  ↓
BC547 transistor stages
  ↓
Switching action
  ↓
Buzzer ON + LED ON

6. Applications
1. Home Automation

IR obstacle detectors can be used to detect the presence of people or objects and trigger automatic lighting or other systems.

2. Security Systems

The detector can be used as a simple sensing element to trigger an alarm when an object enters a monitored area.

3. Drones

Obstacle detection can help drones identify objects in their flight path and avoid collisions.

4. Robots

The detector can be used in robots to identify obstacles and support basic obstacle-avoidance functions.

5. Assistive Devices

Obstacle detection can be incorporated into assistive devices to help visually impaired users identify nearby objects.

6. Cars and Vehicles

Similar sensing concepts can be used for parking assistance and obstacle detection systems.

7. Automatic Doors

Obstacle detection can be used to detect people or objects near an automatic door and prevent the door from closing.

7. Key Concepts Demonstrated

This project provides practical understanding of:

Infrared transmission
Infrared reflection
Photodiode operation
Sensor interfacing
Transistor switching
Signal amplification
LED indication
Buzzer-based alert systems
Basic electronic circuit design

8. Project Demonstration

Add your demonstration video here:

https://drive.google.com/file/d/1oochDgu6kWrp4HVbmb640wg-DK79d3Be/view?usp=drive_link)

9.Future Improvements
The basic circuit can be extended by:

Adding a microcontroller such as Arduino or ESP32.
Displaying the detected distance.
Controlling a robot based on obstacle detection.
Adding multiple IR sensors for detection in different directions.
Adding wireless monitoring.
Using ultrasonic sensors for more accurate distance measurement.
Developing automatic obstacle avoidance.

 10.Conclusion

This project demonstrates a simple and low-cost method of detecting nearby obstacles using infrared transmission and reflection.
The IR LED acts as the transmitter, while the photodiode detects reflected infrared radiation from an obstacle. The signal is processed using BC547 transistor stages, which activate the buzzer and LED when an obstacle is detected.
The project provides a practical introduction to sensors, photodiodes, transistor switching, and electronic detection systems.
