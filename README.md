# mpu6050-zephyr
MPU6050 I2C Interface using Zephyr RTOS

MPU6050-Zephyr is an embedded software project for interfacing the MPU6050 6-axis IMU sensor with an nRF52840 DK (or any Zephyr-compatible board) using I2C protocol in Zephyr RTOS. It reads accelerometer and gyroscope data and logs them with Zephyr’s built-in logging system.

Features
1. Reads accelerometer and gyroscope data
2. Uses Zephyr RTOS I2C API for communication
3. Formatted logging with Zephyr’s logging system
4. Supports nRF52840 DK and other Zephyr-compatible boards

Table of Contents
1. Hardware requirements
2. Pin connections
3. Project structure
4. Installation and setup
5. Data output example

1. Hardware Requirements
   A Zephyr-supported development board like nRF52840 DK is required. The MPU6050 sensor module is used for measuring acceleration and rotation. To establish an I2C connection, 
   connect the SDA and SCL lines to the respective pins on the development board. Power the MPU6050 using a 3.3V or 5V supply.

2. Pin Connections
   Connect the VCC pin of the MPU6050 to the 3.3V or 5V pin on the development board. Connect the GND pin to the ground. The SDA and SCL pins should be connected to the     
   appropriate I2C pins on the development board, such as P0.26 for SDA and P0.27 for SCL on the nRF52840 DK.

3. Project Structure

   mpu6050-zephyr
   1. Main application (I2C communication)
   2. MPU6050 driver implementation
   3. MPU6050 driver header file
   4. Zephyr build configuration
   5. Zephyr project settings
   6. Project documentation
   7. Board-specific configurations

4. Installation and Setup
   ## Installation and Setup

i. Install the required software, including Zephyr SDK and nRF Connect SDK.  

ii. Clone the repository using the following command:  
   ```sh
   git clone https://github.com/yourusername/mpu6050-zephyr.git

   
