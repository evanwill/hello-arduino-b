---
title: 1.0 - Introducing Arduino UNO 
nav: Intro
gallery: true
---

Meet your *microcontroller*!

{% include gallery-figure.html alt="arduino board with parts labelled" img="arduino_intro1.jpg" %}

[Arduino UNO](https://www.arduino.cc/en/Main/ArduinoBoardUno) is an easy to use prototyping board based on **open-source** hardware and software. It can be programmed using Arduino's basic [language](https://www.arduino.cc/en/Reference/HomePage) to create interactive physical computing projects. 

> "Arduino was born at the Ivrea Interaction Design Institute as an easy tool for fast prototyping, aimed at students without a background in electronics and programming. " -- Learn more from the [Arduino Guide](https://www.arduino.cc/en/Guide/Introduction)

For examples and inspiration check out the [Project Hub](https://create.arduino.cc/projecthub).

# 1.1 - Breadboard 

That white thing attached to your UNO? Its a solderless breadboard!

{% include gallery-figure.html alt="Solderless breadboard with parts labelled" img="breadboard.jpg" %}

Breadboard make it easy to create circuits without soldering any wires together. 
The connection is made by inserting wire into the tiny holes: 

- Each pin hole on a `Rail` is connected vertically.
- Each pin hole in a `Row` is connected horizontally. 
- A `Split` runs down the middle dividing the board in two.

# Inputs & Outputs

Arduino is designed to make interactive projects. 
This means it uses sensors to get input from the world, and responds by controlling actuators / outputs.
Uno does not have any built in sensors or actuators, you connect them to the boards pins.

Example sensors:
- button
- potentiometer (dial)
- temperature sensor
- accelerometer (motion sensor)
- photoresistor (light sensor)

Example outputs:
- LED (light)
- piezo buzzer (sound) 
- Servo motor, DC motor (motion)
