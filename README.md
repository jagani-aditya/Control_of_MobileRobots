# Sliding Mode Control

## Project Desciption

### 1. Mobile Robot Simulator
The programming exercises use a simulated version of a robot called the QuickBot. The simulated QuickBot is equipped with five **infrared (IR) range sensors**, of which three are located in the front and two are located on its sides. The simulated QuickBot has a two-wheel difierential drive system (two wheels, two motors) with a wheel encoder for each wheel.

### 2. Differential-Drive, Odometry, and IR
The purpose of this is to implement the functions for the robot to **move and sense**.

    * Transform the outputs of our controllers to the control inputs of the mobile robot.
    * Keep track of where the robot is located.
    * Convert raw sensor values to distances.

### 3. Go-to-Goal PID Controller
The purpose of this is to implement a **go-to-goal PID controller**.

    * Implement the proportional, integral, and derivative terms of the controller.
    * Adjust the gains for performance.

### 4. Obstacle Avoidance
The purpose of this is to **avoid any obstacles** near the robot.

    * Transform the IR distance to a point in the robot’s coordinate frame.
    * Transform this point from the robot’s coordinate frame to the world coordinate frame.
    * Compute a vector that points away from any obstacles.
    
### 5. Arbitration
Utilizing two arbitration techniques, **blending and hard switching** - to drive to a goal while avoiding obstacles.

    * Blend go-to-goal and avoid-obstacle vectors in one controller.
    * Switch between go-to-goal and avoid-obstacle controllers separately.
    * Use the blended controller as an intermediary.

### 6. Following Walls
Adding a **new controller** to follow walls.

    * Estimate a section of a wall (obstacle) using the IR sensors.
    * Compute a vector tangential to the wall and perpendicular to the wall.
    * Combine the two vectors and steer in the direction of this new vector.
    
### 7. Navigation
In this module we achieve navigation through the obstacle course:

    * Is the robot making progress towards the goal?
    * Should the robot follow the wall to the right or the left?
    * If the robot is in state “A” and event “2” becomes true, then to which state should the robot switch?
    
### Results

![Autonomous Mobile Robot Navigation using Sliding Control](/Media/Controls1.gif)

## Platform

## Implementation
