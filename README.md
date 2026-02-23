ESP32 Gesture-Controlled Door (Prototype)
Overview

This project is a small prototype of a gesture-controlled door mechanism using an ESP32-CAM and a servo motor.

A TinyML model trained with Edge Impulse runs directly on the ESP32 to detect two hand gestures and rotate the servo accordingly.

This project was built to explore embedded AI and basic hardware control on microcontrollers.

Hardware

ESP32-CAM

SG90 Servo Motor

External 5V power supply

Breadboard and jumper wires

Gestures

Closed fist → Open door

Open hand → Close door

The model runs entirely on-device (no cloud connection).

How It Works

The ESP32-CAM captures an image.

The image is passed to the embedded Edge Impulse model.

The model outputs a prediction score.

If the confidence is above a threshold, the servo rotates.
