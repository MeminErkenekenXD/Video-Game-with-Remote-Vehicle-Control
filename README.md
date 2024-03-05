# Video-Game-with-Remote-Vehicle-Control
# Overview
This project is a video game where you remote control a car from your computer with Wi-Fi communication. Using your gamepad as a controller. You also get live camera feedback from the car which you see on your game screen. The goal is to complete a lap by passing 3 checkpoints and return to the first checkpoint.You can create tracks using checkpoints although the car can also be controlled without them.

Setting up the connections and passing through the first checkpoint to start the lap.

![gif 1](https://github.com/MeminErkenekenXD/Video-Game-with-Remote-Vehicle-Control/assets/97636236/7c259db7-078f-4397-81ef-7448464a99b8)

# Why Use Gamepad 
In wi-fi or radio controlled vehicles, the controls are usually provided by simple control
schemes such as forward, backward, right, left, forward right, forward left, backward
right and backward left. Such shallow control schemes are insufficient to control the
vehicle with the desired accuracy and precision. In this project we use a game
controller (gamepad) to control the velocity and direction of the vehicle exactly as we
want.

![gif2](https://github.com/MeminErkenekenXD/Video-Game-with-Remote-Vehicle-Control/assets/97636236/848b1aa5-bc76-43b1-b858-5393207646a0)

Demonstration of trigger and analog controlled car. The car will slowly starts moving if you barely pressing the trigger and it will go max speed when fully held down. So you can control how fast you want the car to go by adjusting the trigger, similiar to how real throttles work. The same logic applies to steering with analog stick as well. The car will turn sharper as you tilt the stick more.

# Components

For building the car ; <br>

![22](https://github.com/MeminErkenekenXD/Video-Game-with-Remote-Vehicle-Control/assets/97636236/617cd313-cf5c-486b-9dbf-6fbf2d9c3b1f)


- **ESP32 DevKit V1 Microcontroller** : Recieves and send signals to Unity . Drives the car with motor driver.
- **L298N Motor Driver** : Component required to drive the DC motors.
- **2 x DC Motor With Reduction** : Motors to give power to wheels to drive and steer the car.
- **2 x Wheel** : Lightweight plastic-silicon alloy wheel.
- **2 x ASPILSAN INR18650A28 Batteries** : Batteries to power up the ESP32 thus the motors.
- **HC-SR04** : Distance sensor to determine upon passing a checkpoint.
- **Body for Car** : Self-explanatory.

Custom made handle to hold the phone, the spring strengthens the grip so the phone doesn't fall off on bumpy terrains or high speed turns.

![1](https://github.com/MeminErkenekenXD/Video-Game-with-Remote-Vehicle-Control/assets/97636236/9ed55a85-e670-47c5-9a36-8cc7389daef9)

Hand made checkpoints;

![checkpoints](https://github.com/MeminErkenekenXD/Video-Game-with-Remote-Vehicle-Control/assets/97636236/54f31f1b-b1db-4f91-a660-1795c95a7957)

For developing the game ; <br>

- **Arduino IDE** : ESP32 is being coded on Arduino IDE.
- **OBS Studio / OBS Ninja** : OBS is used for taking your phone cameras view (which should be set up on the car) into Unity game screen.
- **Unity 3D** : Game is developed on Unity Engine. Input system as well as communicating with the car (using ESP32's Wi-Fi support).There are extra mechanics in addition to controlling the car such as a lap time system and nitrous/boost system.
