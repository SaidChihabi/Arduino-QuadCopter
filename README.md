# Arduino Quadcopter

Welcome to the Arduino Quadcopter GitHub repository! This repository contains the source code and necessary files for building and programming an Arduino-based quadcopter using an Arduino Uno, MPU 6050 gyro accelerometer, LiPo 11.1V battery, four 30A ESCs, 2200KV brushless motors, and the "Fleshy" receiver and transmitter code from Loop Brokking.

## Project Overview

This project aims to provide you with the necessary resources to build and program your own quadcopter using Arduino. By utilizing the MPU 6050 gyro accelerometer, the quadcopter can detect its orientation and make adjustments to maintain stability during flight. The ESCs control the speed of the brushless motors, allowing the quadcopter to maneuver and hover in the air. The included receiver and transmitter code enables wireless control of the quadcopter.

## Repository Structure

The repository is structured as follows:

- **`setup.ino`**: This Arduino sketch contains the setup code that initializes the necessary components and establishes communication with the MPU 6050 gyro accelerometer and ESCs. It also includes the receiver and transmitter setup.
- **`esc-calibration.ino`**: This Arduino sketch assists in calibrating the ESCs. It provides a simple interface to calibrate the minimum and maximum throttle values for each ESC, ensuring proper motor control.
- **`flight-controller.ino`**: This is the main flight controller code. It implements the control algorithms required to stabilize the quadcopter, read sensor data from the MPU 6050, and control the ESCs and motors based on the user input.

## Getting Started

To get started with this project, follow these steps:

1. Clone or download this repository to your local machine.
2. Open the Arduino IDE (Integrated Development Environment) and ensure you have the necessary libraries installed. The required libraries are:
   - `I2Cdev` - Enables communication with the MPU 6050 sensor.
   - `MPU6050` - Provides functions to read data from the MPU 6050 sensor.
   - Any additional libraries required by the receiver and transmitter code.
3. Connect the Arduino Uno to your computer using a USB cable.
4. Open the `setup.ino` sketch in the Arduino IDE and upload it to the Arduino Uno.
5. Follow the necessary hardware connections and configurations as outlined in the project documentation.
6. Open the `esc-calibration.ino` sketch and upload it to the Arduino Uno. Follow the on-screen instructions to calibrate the ESCs.
7. Finally, open the `flight-controller.ino` sketch, customize the control algorithms or parameters if desired, and upload it to the Arduino Uno.
8. Ensure the LiPo 11.1V battery is connected and secure.
9. Power on the quadcopter and enjoy flying!

## Contributing

Contributions to this project are welcome. If you find any issues, have suggestions for improvements, or want to add new features, please feel free to submit a pull request. However, please ensure that any changes align with the project's goals and maintain its overall stability and usability.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code for personal and commercial purposes. Please refer to the license file for more details.

## Acknowledgments

This project would not have been possible without the following resources:

- Loop Brokking's receiver and transmitter code, which forms the basis for wireless control.
- The `I2Cdev` and `MPU6050` libraries for interfacing with the MPU 6050 gyro accelerometer.

We are grateful for the hard work and dedication of the developers who
