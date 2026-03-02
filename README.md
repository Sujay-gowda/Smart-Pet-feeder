# Smart-Pet-feeder
An Smart Pet Feeding real time system using a servo-controlled dispenser and ultrasonic sensor for scheduled feeding and food-level monitoring.


## Introduction

The Smart Automatic Pet Feeder is an automated pet care system developed to feed pets at the correct time without human intervention. The system is designed for pet owners who may be busy, travelling, or away from home and cannot always maintain a regular feeding schedule.

The feeder uses a programmable controller, a motorized dispensing mechanism, and sensors to provide controlled portions of food. It also connects to a mobile application, allowing the user to monitor and control feeding remotely.

---

## Objective

The main objective of this project is to automate the pet feeding process and ensure pets receive meals on time while also informing the owner about the food availability inside the feeder.

---

## Problem Statement

Many pet owners forget feeding times due to college, work, or daily activities. Inconsistent feeding affects the pet’s health and routine. Manual feeding also makes it difficult for owners to leave pets alone for long durations.

This system solves the problem by providing automatic feeding, remote control, and food level monitoring.

---

## Key Features

* Automatic feeding at scheduled times
* Manual feeding through mobile application
* Servo motor controlled food dispensing
* Ultrasonic sensor based food level detection
* Low food notification alerts
* Remote monitoring and control

---

## System Architecture

The system is built around an ESP32 microcontroller. The controller connects to Wi-Fi and communicates with a mobile application.

The servo motor controls the opening and closing of the food outlet.
The ultrasonic sensor measures the distance between the sensor and the food level inside the container.

When the feeding time arrives or when the user presses the feed button on the mobile app, the controller rotates the servo motor to release food and then closes it automatically.

---

## Mobile Application (Blynk)

The feeder is connected to a mobile app using the Blynk platform. The mobile application allows the user to:

* Manually trigger feeding
* Automate feeding schedules
* Receive feeding reminders
* Get low food notifications
* Monitor system status remotely

This enables the owner to control the feeder from anywhere using the internet.

---

## Working Principle

1. The ESP32 connects to Wi-Fi and the mobile application.
2. Feeding can be triggered either by schedule or by pressing the feed button in the app.
3. The servo motor rotates and opens the food container.
4. A fixed portion of food is dispensed into the bowl.
5. The servo returns to its original position and closes the outlet.
6. The ultrasonic sensor measures the food level inside the container.
7. If the food level is low, a notification is sent to the user’s phone.

---

## Hardware Components

* ESP32 Microcontroller
* Servo Motor
* Ultrasonic Sensor (HC-SR04)
* Power Supply
* Food storage container
* Feeding bowl

---

## Software Used

* Arduino IDE
* Embedded C / Arduino Framework
* Blynk IoT Platform
* Wi-Fi Communication Libraries

---

## Food Level Monitoring

The ultrasonic sensor continuously measures the distance between the sensor and the food surface.
If the measured distance increases beyond a threshold value, the system determines that the feeder is nearly empty and sends an alert notification to the user.

---

## Applications

* Pet care automation
* Smart home systems
* Remote monitoring systems
* Animal care management

---

## Advantages

* Ensures timely feeding
* Reduces owner dependency
* Prevents overfeeding
* Allows remote control
* Provides food refill alerts

---

## Future Improvements

* Portion size customization
* Camera monitoring
* Multiple pet profiles
* Feeding history tracking

