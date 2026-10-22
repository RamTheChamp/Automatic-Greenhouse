# 🌱 IoT-Based Automatic Greenhouse System

An ESP32-based smart greenhouse system that monitors temperature, humidity, soil moisture, and light intensity. It automatically controls a fan, water pump, and bulb using sensor readings, while MQTT enables remote monitoring and manual control.

## ✨ Features

- 🌡️ Monitors temperature and humidity using DHT11.
- 💧 Automatically controls the water pump based on soil moisture.
- 💨 Controls the fan based on temperature.
- 💡 Automatically switches the bulb based on light intensity.
- 📡 Publishes sensor data through MQTT over Wi-Fi.
- 🎮 Supports remote manual control of relays using MQTT messages.
- 🖥️ Displays real-time sensor readings on a 16×2 I2C LCD.

## 🧰 Components Used

- ESP32
- DHT11 Temperature and Humidity Sensor
- Soil Moisture Sensor
- LDR (Light Sensor)
- 3-Channel Relay Module
- DC Fan, Water Pump, and Bulb
- 16×2 I2C LCD
- Wi-Fi Network and MQTT Broker

## ⚙️ Technologies

`ESP32` `Arduino IDE` `C++` `MQTT` `Wi-Fi` `IoT` `Embedded Systems`

## 🔄 Working Principle

The ESP32 reads sensor data and publishes it to MQTT topics. Based on predefined thresholds, it automatically controls the fan, pump, and bulb. An MQTT control topic also allows manual operation of these devices, with manual overrides taking priority over automatic control.

## 🚀 Getting Started

1. Install the required Arduino libraries: `DHT sensor library`, `LiquidCrystal_I2C`, and `PubSubClient`.
2. Configure your Wi-Fi credentials and MQTT broker IP address.
3. Connect the sensors, LCD, and relay module to the configured ESP32 GPIO pins.
4. Upload the code using Arduino IDE.
5. Connect an MQTT client to monitor sensor data and control the relays.

## 🔮 Future Improvements

- 📊 Historical sensor data visualization.
- 🔔 Alerts for extreme temperature or low soil moisture.
- ☁️ Cloud-based monitoring and data storage.

---

**Built with 🌱 for smarter, automated, and efficient greenhouse management.**

⭐ If you like this project, consider giving the repository a star!
