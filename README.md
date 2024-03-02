# Video-Game-with-Remote-Vehicle-Control
# Overview
This project is a video game where you remote control a car from your computer with Wi-Fi communication. Using your keyboard or gamepad as a controller. You also get live camera feedback from the car which you see on your game screen. The goal is to complete a lap by passing 3 checkpoints and return to the first checkpoint.You can create tracks using checkpoints although the car can also be controlled without them.

# Why Use Gamepad 
In wi-fi or radio controlled vehicles, the controls are usually provided by simple control
schemes such as forward, backward, right, left, forward right, forward left, backward
right and backward left. Such shallow control schemes are insufficient to control the
vehicle with the desired accuracy and precision. In this project we use a game
controller (gamepad) to control the velocity and direction of the vehicle exactly as we
want.

# Components

For building the car ; <br>

- **ESP32 DevKit V1 Microcontroller** : Recieves and send signals to Unity . Drives the car with motor driver.
- **L298N Motor Driver** : Component required to drive the DC motors.
- **2 x DC Motor With Reduction** : Motors to give power to wheels to drive and steer the car.
- **2 x Wheel** : Lightweight plastic-silicon alloy wheel.
- **2 x ASPILSAN INR18650A28 Batteries** : Batteries to power up the ESP32 thus the motors.
- **HC-SR04** : Distance sensor to determine upon passing a checkpoint.
- **Body for Car** : Self-explanatory.

For developing the game ; <br>

- **Arduino IDE** : ESP32 is being coded on Arduino IDE.
- **OBS Studio / OBS Ninja** : OBS is used for taking your phone cameras view (which should be set up on the car) into Unity game screen.
- **Unity 3D** : Game is developed on Unity Engine. Input system as well as communicating with the car (using ESP32's Wi-Fi support).There are extra mechanics in addition to controlling the car such as a lap time system and nitrous/boost system.
