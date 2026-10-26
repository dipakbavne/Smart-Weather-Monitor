# Smart Weather Monitor — Pin Connections

## 1. Hardware Connections

| Component          | Signal               | ESP32 Pin / Interface |
| ------------------ | -------------------- | --------------------- |
| DHT11 Sensor       | Data                 | GPIO 4                |
| BMP180 Sensor      | SDA                  | I2C SDA               |
| BMP180 Sensor      | SCL                  | I2C SCL               |
| Rain Sensor        | Digital Output       | GPIO 27               |
| 16x2 I2C LCD       | SDA                  | I2C SDA               |
| 16x2 I2C LCD       | SCL                  | I2C SCL               |
| Rain Indicator LED | Control              | GPIO 15               |
| Status LED         | Control              | GPIO 13               |
| DFPlayer Mini      | Serial Communication | GPIO 16 and GPIO 17   |

## 2. Communication Interfaces

### I2C Communication

The BMP180 sensor and 16x2 I2C LCD use the I2C communication interface to communicate with the ESP32.

The actual SDA and SCL pins should be verified from the project firmware.

### UART Communication

The DFPlayer Mini communicates with the ESP32 using UART serial communication.

The TX and RX connections should be checked against the actual hardware wiring and firmware configuration.

## 3. Working Description

* The DHT11 measures temperature and humidity.
* The BMP180 measures atmospheric pressure.
* The rain sensor detects rain through its digital output.
* The LCD displays the sensor readings.
* The ESP32 sends sensor data to ThingSpeak over Wi-Fi.
* The DFPlayer Mini provides configured voice alerts.
* LEDs indicate selected system or weather conditions.

## 4. Important Notes

* Verify all GPIO assignments against the final firmware.
* Confirm the I2C address of the LCD from the project configuration.
* Check the operating voltage requirements of all components.
* Ensure that ESP32 GPIO pins are not exposed to unsafe voltage levels.
* Disconnect the power supply before changing hardware connections.

## 5. Verification

All pin connections should be checked against the actual circuit and tested before operating the system.

This document should be updated whenever the hardware wiring or firmware pin assignments change.

