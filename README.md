# 🌦️ Smart Weather Monitor

### Integrating Sensors & Voice Reporting Features

An ESP32-based Embedded Systems and IoT project for monitoring environmental conditions, displaying sensor readings, uploading data to the cloud, and providing voice alerts.

---

## 📌 Project Overview

The **Smart Weather Monitor** is designed to monitor environmental parameters using multiple sensors and an ESP32 microcontroller.

The system measures temperature, humidity, atmospheric pressure, and rain status. Sensor readings are displayed on a 16×2 I2C LCD and uploaded to the ThingSpeak IoT cloud platform for remote monitoring.

A DFPlayer Mini audio module provides voice alerts based on predefined environmental conditions, while LEDs indicate selected system or weather statuses.

This project demonstrates practical applications of embedded programming, sensor interfacing, wireless communication, and IoT-based environmental monitoring.

---

## ✨ Key Features

* 🌡️ Temperature and humidity monitoring
* 🌬️ Atmospheric pressure measurement
* 🌧️ Rain detection using a digital rain sensor output
* 📟 Real-time sensor readings on a 16×2 I2C LCD
* ☁️ Cloud-based monitoring using ThingSpeak
* 🔊 Voice alerts using the DFPlayer Mini audio module
* 💡 LED indicators for selected conditions
* 📶 Wireless data transmission using ESP32 Wi-Fi connectivity

---

## 🛠️ Hardware Components

| Component               | Purpose                                |
| ----------------------- | -------------------------------------- |
| ESP32 Development Board | Main controller and Wi-Fi connectivity |
| DHT11 Sensor            | Temperature and humidity measurement   |
| BMP180 Sensor           | Atmospheric pressure measurement       |
| Digital Rain Sensor     | Rain detection                         |
| 16×2 I2C LCD            | Local display of readings              |
| DFPlayer Mini           | Audio and voice alerts                 |
| LEDs                    | Visual status indication               |
| Speaker                 | Audio output                           |
| Connecting Wires        | Electrical connections                 |

---

## 💻 Software and Technologies

* **Programming:** Embedded C/C++ using the Arduino framework
* **IDE:** Arduino IDE
* **Microcontroller:** ESP32
* **Communication:** I2C, UART, and Wi-Fi
* **IoT Platform:** ThingSpeak
* **Sensor Interfacing:** DHT11, BMP180, and digital rain sensor

---

## ⚙️ Working Principle

1. The ESP32 initializes the connected sensors and output modules.
2. The DHT11 measures temperature and humidity.
3. The BMP180 measures atmospheric pressure.
4. The digital rain sensor provides rain-status information.
5. The ESP32 processes the readings and displays them on the LCD.
6. The system uploads configured sensor data to ThingSpeak over Wi-Fi.
7. The DFPlayer Mini provides voice alerts when configured conditions are met.
8. LEDs indicate selected weather conditions or system status.

---

## 🚨 Alert Conditions

The system uses configurable thresholds for environmental monitoring.

| Parameter            | Configured Condition                                   |
| -------------------- | ------------------------------------------------------ |
| Temperature          | Above 40°C                                             |
| Humidity             | Above 80%                                              |
| Atmospheric Pressure | Monitored against the configured range of 990–1025 hPa |
| Rain                 | Detected using the digital output of the rain sensor   |

**Note:** These are project-defined thresholds, not official severe-weather warning limits.

---

## 🔌 Hardware Connections

The main ESP32 connections used in the project are documented separately.

See [`hardware/pin_connections.md`](hardware/pin_connections.md) for the pin connection details.

---

## 📂 Repository Structure

```text
Smart-Weather-Monitor/
│
├── README.md
├── firmware/
│   └── Smart_Weather_Monitor.ino
│
├── hardware/
│   ├── circuit_diagram.png
│   └── pin_connections.md
│
├── images/
│   ├── project_setup.jpg
│   ├── lcd_output.jpg
│   └── thingspeak_dashboard.jpg
│
└── docs/
    └── project_report.pdf
```

*Note: Some files may be added as documentation and project images become available.*

---

## 📸 Project Demonstration

Project photographs and screenshots will be added here.

* **Hardware Setup:** Complete assembled project.
* **LCD Output:** Sensor readings displayed on the LCD.
* **ThingSpeak Dashboard:** Cloud visualization of uploaded data.

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

* ESP32 programming and embedded systems development
* Interfacing multiple sensors with a microcontroller
* I2C and UART communication
* Wi-Fi-based data transmission
* IoT cloud integration using ThingSpeak
* Implementing sensor-based alerts
* Hardware debugging and system integration

---

## 🔮 Future Improvements

* Add historical data analysis and weather trends.
* Improve the cloud dashboard and data visualization.
* Integrate additional environmental sensors.
* Develop a mobile-friendly monitoring interface.
* Add more advanced alerting and notification features.

---

## 🎯 Applications

* Environmental condition monitoring
* Educational embedded systems projects
* IoT and sensor-interfacing demonstrations
* Local weather observation and data logging

---

## 👨‍💻 Project Category

**Embedded Systems | Internet of Things (IoT) | ESP32 | Sensor Interfacing**

Developed as a hands-on electronics engineering project to explore embedded programming and IoT-based environmental monitoring.
