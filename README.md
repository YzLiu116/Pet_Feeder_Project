# Automated Pet Feeder

## Overview
The Automated Pet Feeder is a controller-based system designed to feed pets at scheduled times safely.  
It ensures pets receive the right amount of food on time while also monitoring food availability and consumption.

## Features
1. **Scheduled feeding** using a Real-Time Clock module
2. **Food container level detection** to prevent failed feedings
3. **Bowl weight monitoring** before and after feeding
4. **Servo motor control** for accurate portion dispensing
5. **Alert notifications** when there is no food, the pet has not eaten, or dispensing fails

## System Workflow
1. **Time Check** Continuously monitor current time from RTC and compare it to feeding schedule.
2. **Pre-feeding Check** Confirm hopper contains enough food before dispensing.
3. **Food Dispensing** Activate servo rotating motor to release a portion into the bowl.
4. **Dispense Verification** Use bowl weight sensor to confirm successful dispensing.
5. **Eating Monitoring** Wait a set time (10 mins), then check if the pet has eaten.
6. **Alerts** Send notifications for empty container, failed dispensing, or uneaten food.

## Hardware Components
- Microcontroller (Arduino)
- Real-Time Clock (for detecting time)
- Container Level Sensor (for checking food remain amount)
- Load Cell with Amplifier (for bowl weight)
- Servo Rotating Motor (for food supply)
- LED/Buzzer or Network Module (for alerts)

## Author
Yizheng Liu
