# Upset Fowl

## Overview

"**Upset Fowl**" is a simple C++ console game that simulates a projectile motion scenario. The objective is to hit the "**Mean Swine**" by launching an "**Upset Fowl**" using a specified angle and velocity. The program calculates the trajectory of the fowl and determines if it hits the swine, giving the player up to four attempts.

## Features

- Simulates projectile motion with gravity.
- Randomly generates the target distance (Mean Swine) for each game.
- Allows user input for launch angle and velocity.
- Provides feedback on whether the target was hit or missed.
- User gets up to four attempts to hit the target.

## Code Structure

### Constants

- **`pi`**: Value of π for converting degrees to radians.
- **`grav`**: Acceleration due to gravity on Earth (9.8 m/s²).

### Functions

- **`void Trajectory(double t, double a, double v, double& x, double& y)`**: 
  - Updates the x and y coordinates of the projectile at time `t` based on angle `a`, velocity `v`, and gravity.
  
- **`double DegToRad(double deg)`**: 
  - Converts an angle from degrees to radians.
  
- **`void PrintUpdate(double t, double x, double y)`**: 
  - Prints the time, x, and y coordinates of the projectile.
  
- **`void PrintIntro()`**: 
  - Prints the introduction to the game.
  
- **`void GetUsrInpt(double swineX, double fowlAngle, double fowlVel)`**: 
  - Prompts the user to input the launch angle and velocity.
  
- **`double LaunchFowl(double fowlAngle, double fowlVel)`**: 
  - Simulates the flight of the projectile and returns its final x-coordinate.
  
- **`bool DtrmnIfHit(double fowlLandingX, double swineX)`**: 
  - Determines whether the fowl hit the swine based on the landing position.

## How to Play

1. Run the program.
2. The game will display an introductory message.
3. The program will generate a random distance for the Mean Swine.
4. Enter the desired launch angle (in degrees) and velocity (in meters per second) when prompted.
5. The program will calculate the flight path of the Upset Fowl and determine if it hits the Mean Swine.
6. You have up to four attempts to hit the target. The game ends if you succeed or exhaust all attempts.

## Example

Welcome to Upset Fowl!
The objective is to hit the Mean Swine by launching an Upset Fowl.

The Mean Swine is 150 meters away.
Enter fowl launch angle (deg): 45
Enter fowl launch velocity (m/s): 30

Time 1 x = 21 y = 14
Time 2 x = 42 y = 24
Time 3 x = 63 y = 31
Time 4 x = 84 y = 34
Time 5 x = 105 y = 33
Time 6 x = 126 y = 29
Time 7 x = 147 y = 21
Time 8 x = 168 y = 10
Time 9 x = 189 y = -6
Missed'em...


## Dependencies

- C++ Standard Library

## Compilation

To compile the program, use a C++ compiler like `g++`:


```sh
g++ -o upset_fowl upset_fowl.cpp -std=c++11


```
---
   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0
---
## Developed by Cedric Nartey

