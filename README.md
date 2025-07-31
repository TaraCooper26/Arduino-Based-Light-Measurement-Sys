# Arduino-Based-Light-Measurement-Sys
# Automatic Blinds Controlled by Light Sensor

An Arduino-based system that automatically opens/closes window blinds based on ambient light levels using a photoresistor and micro servo.

## Team Project Info
- Course: ME 3113 - Measurements & Instrumentation
- Team Project
- University: UTSA
- Semester: Spring 2025

## Components Used
- Ardunino Uno R3
- Photoresistor (LDR)
- Micro Servo Motor
- LCD Display (16x2)
- 10kΩ resistor
- Potentiometer
- Capacitor (100 µF)
- Cardboard test chamber + flashlight
- Excel for data logging

## 🧠 How It Works
- A **photoresistor** reads light intensity.
- Arduino calculates **voltage** output using a voltage divider.
- Based on voltage threshold:
  - If dark: servo rotates to 0° (blinds close)
  - If bright: servo rotates to 180° (blinds open)
- Real-time voltage shown on **LCD display**

## 📊 Results & Analysis
- Exponential relationship between lux and output voltage  
- Voltage converted to lux:  
  `Lux = 2.7189 * exp(2.7675 * Voltage)`
- Accuracy verified using Light Meter app
