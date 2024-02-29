# Lab 4: Microcontrollers, Sensors and Actuators


## Overview and Motivation
This week we'll explore...

## Materials

## Part 1: Exploration: Buzzer

The buzzer is a device that emits a sound whose pitch is based on how fast voltage changes from +5V to 0V and back, also known as the frequency of the signal. This is demonstrated through the square wave generator on the left of the breadboard. When we change the signal to 5hz, this means it is oscillating from +5V to 0V 5 times in 1 second. With only a breadboard, the buzzer is easy to understand. However, we can also use an Arduino to further control its behavior.

<img width="413" alt="image" src="https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/adf820df-50cf-42f8-8842-f4f7706d7760">

This is the code for the Arduino to control the buzzer. We first indicate the "Buzzer" pin, or the output of the Arduino going into the buzzer. this will serve as a substitute to our square function generator. We then run a for loop, where the signal outputted by the arduino will go from High to Low, with p delay in between. To make the pitch go higher, we can reduce p, thus increasing the frequency of the voltage oscillations going into the buzzer. To make the pitch go lower, we can instead reduce p.


## Part 2: Exploration: Ultrasonic Sensor

#### Goal

#### Steps

#### Testing


## Part 4: Design: Distance detector with buzzer and ultrasonic sensor

#### Goal

#### Steps

#### Testing

## Conclusion




