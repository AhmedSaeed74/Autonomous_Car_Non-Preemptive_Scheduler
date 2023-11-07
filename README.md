# Real-Time Operating System Scheduler for Autonomous Car

## Project Overview

Real-time operating systems (RTOS) involve managing tasks that serve specific functionalities. The project's primary goal is to implement a non-preemptive scheduler that switches between different tasks. These tasks are integral to the operation of an autonomous car equipped with sensors and motors.

### Description

The autonomous car is equipped with the following components:

1. Two Photo-Resistors.
2. One Ultrasonic Sensor Module HC-SR04.
3. On-board Temperature sensor.
4. One LCD.
5. Four motors + Two motor drivers.

The motors can be controlled using on-board switches. When started, the car moves toward the direction with the highest illumination. Temperature, light sensor readings, and elapsed time are displayed on the LCD.

If the car detects an obstacle within 10 centimeters, the ultrasonic sensor triggers a response. The car first reverses and then rotates by 90 degrees.

The scheduler is responsible for managing these tasks in a non-preemptive manner.

### Project Structure

The project is organized into the following components:

- `scheduler.c` and `scheduler.h`: Implements a non-preemptive scheduler. Supports multiple tasks with a predefined macro "NUM_OF_TASKS."

- `tasks.c` and `tasks.h`: Tasks include functions for swinging the car based on light sensor readings, displaying information on the LCD, and avoiding obstacles based on ultrasonic sensor data.

- `main.c`: The main function initializes and sets up hardware, creates tasks, and starts the scheduler.

### Project Levels

The project is structured into different layers, ensuring that lower layers don't depend on upper layers. These layers include files for tasks, the scheduler, and various hardware components.


Please click the link to make sure everything works perfectly and passes all tests without any problems.

https://drive.google.com/file/d/1IX0HTextuvzLCd_k78c0gHB6z56Ht03O/view?usp=drive_link

## Contributing

Contributions and enhancements to this project are welcome. Feel free to fork the repository and create pull requests to improve the scheduler and the autonomous car's functionality.

