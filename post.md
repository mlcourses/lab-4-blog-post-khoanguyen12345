# Lab 4: Microcontrollers, Sensors and Actuators

## Overview and Motivation
This week, we explored actuators, or circuit components that interact with real life elements. We will then use these to create a distance detector that changes pitch based on how far an object is away from our sensor. The two actuators we will use are the ultrasonic distance sensor and the buzzer.

Actuators are important because they "actualize" our circuit. It means our circuits can have real world effects, either by reading outputs in the real world (ultrasonic sensor) or by playing a sound (buzzer). Therefore, it is important to explore the role of actuators in circuits. Plus, they are realy cool!

## Materials
1. PB-503 (breadboard)
2. Electrical Wires
3. Buzzer
4. Ultrasonic Sensor
5. Arduino Kit
6. Ruler
7. A flat surface (one the ultrasonic sensor can consistently detect)

## Part 1: Buzzer

The buzzer is a device that emits a sound whose pitch is based on how fast voltage changes from +5V to 0V and back, also known as the frequency of the signal. This is demonstrated through the square wave generator on the left of the breadboard. When we change the signal to 5hz, this means it is oscillating from +5V to 0V 5 times in 1 second. With only a breadboard, the buzzer is easy to understand. However, we can also use an Arduino to further control its behavior.

<img width="413" alt="image" src="https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/adf820df-50cf-42f8-8842-f4f7706d7760">

This is the code for the Arduino to control the buzzer. We first indicate the "Buzzer" pin, or the output of the Arduino going into the buzzer. this will serve as a substitute to our square function generator. We then run a for loop, where the signal outputted by the arduino will go from High to Low, with p delay in between. To make the pitch go higher, we can reduce p, thus increasing the frequency of the voltage oscillations going into the buzzer. To make the pitch go lower, we can instead reduce p.

Another way to tone the buzzer using the Arduino is to use the tone() function. The tone() function takes in 2 arguments, the pin number and the an integer (the frequerncy to be set) and sets the frequency of the arduino to that second argument. The tone function has an optional third argument, which can change the duration of the tone from infinite as long as the buzzer is plugged in to a fixed duration. Another option to change the tone is to add a delay and then call another tone function that sets the frequency to another frequency, thus, alternating two different pitches. The code below uses the tone() function:

<img width="252" alt="image" src="https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/c1cfbde1-e663-4666-b13e-9c015859cd07">

These are the videos testing the buzzer with the square function generator and the Arduino:

With square function generator:
https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/05b6322d-1c1f-40bc-8caa-2e20c8304c4f

With arduino:
https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/2604b2b2-c265-4272-ade1-c1edd22e37f4


## Part 2: Ultrasonic Sensor

The ultrasonic sensor emits an ultrasonic wave that reflects off of a surface and "receives" that signal. The time in between is then used to calculate the distance of the surface from the sensor. The code for the sensor can be seen below:

<img width="485" alt="image" src="https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/582a0447-3cbe-4b35-8448-4bcd1805beed">

When a high signal is sent to the ultrasonic sensor, it starts sending out an ultrasonic signal. The low signal puts the ultrasonic sensor on "receiving mode" and so, it would start "sensing" for the signal it sent out. pulseIn() is an Arduino function that takes in two arguments, the first being the pin number and the second being either HIGH or LOW. If it is set to HIGH, it means the Arduino unit will start timing when the signal goes from LOW to HIGH and will stop when the signal goes back to LOW.

This is a video showing the ultrasonic sensor in effect, with a ruler:

https://github.com/mlcourses/lab-4-blog-post-khoanguyen12345/assets/67582698/8d9b2b23-10d3-4768-9e67-57fa3ae7bc9f

## Part 3: Distance detector with buzzer and ultrasonic sensor

#### Goal

#### Steps

#### Testing

## Conclusion




