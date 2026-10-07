# IGNIS X – Intelligent Fire Intelligence System

IGNIS X is an IoT-based intelligent fire detection and emergency monitoring system designed to provide early fire-risk detection, real-time environmental monitoring, local alerts, and remote emergency notifications.

The system combines multiple sensors with an edge controller to analyze environmental conditions and identify potential fire-related events. Instead of relying on a single sensor, IGNIS X uses information from smoke, gas, flame, temperature, humidity, occupancy, and infrared temperature sensors to provide a more comprehensive understanding of the surrounding environment.

## Key Features

- 🔥 Multi-sensor fire detection
- 🌡️ Real-time temperature and humidity monitoring
- 💨 Smoke and gas detection
- 🔥 Flame detection
- 👤 Occupancy/motion detection using PIR
- 🌡️ Non-contact temperature monitoring using MLX90614
- 🚨 Local emergency alerts using buzzer and LEDs
- 📟 Local status display
- 📱 Mobile monitoring using Flutter
- 🔵 Bluetooth Low Energy (BLE) device discovery and configuration
- 📡 Wi-Fi-based telemetry and remote monitoring
- 📶 4G/LTE communication as a future backup channel
- 📡 LoRa-based long-range communication support
- 🤖 Future AI/ML-based anomaly detection and risk prediction
- 📊 Event logging and monitoring

## System Architecture

IGNIS X follows a layered architecture:

1. **Sensing Layer** – Collects data from multiple environmental and occupancy sensors.
2. **Edge Processing Layer** – Processes sensor readings and determines the current safety state.
3. **Local Safety Layer** – Activates the buzzer, LEDs and display during abnormal conditions.
4. **Communication Layer** – Provides BLE, Wi-Fi, 4G/LTE and LoRa communication options.
5. **Backend Layer** – Stores telemetry and emergency events for remote monitoring.
6. **Application Layer** – Provides a Flutter-based interface for monitoring and alerts.
7. **Intelligence Layer** – Provides a foundation for future AI/ML-based fire-risk analysis.

## Hardware

The current prototype consists of a microcontroller-based breadboard implementation with multiple sensor and output modules.

Major components include:

- Arduino UNO – current prototype controller
- ESP32-S3 – target integrated controller
- Smoke sensor
- Gas sensor
- Flame sensor
- DHT22-class temperature/humidity sensor
- PIR motion sensor
- MLX90614 infrared temperature sensor
- OLED/display
- Buzzer
- RGB/status LEDs
- Relay module
- Breadboard and jumper connections

> **Note:** The current physical prototype and the target ESP32-S3 architecture are treated separately. Features that have not yet been experimentally verified are considered planned or future extensions.

## Software

The project can use:

- Arduino/C++ for embedded firmware
- Flutter/Dart for the mobile application
- BLE for local device discovery and configuration
- Wi-Fi for normal telemetry
- MQTT or a suitable realtime backend for communication
- Cloud/database services for event and telemetry storage
- Python/ML frameworks for future intelligent analytics

## Emergency Detection Concept

IGNIS X uses a multi-level safety model:

- **NORMAL** – Environmental conditions are within expected limits.
- **WARNING** – One or more abnormal sensor conditions are detected.
- **EMERGENCY** – Multiple corroborating signals or a validated fire-related condition are detected.
- **SENSOR FAULT** – A sensor produces invalid, unavailable, or abnormal readings.

The system is designed so that local emergency response remains available even when remote communication is unavailable.

## Mobile Application

The planned IGNIS X mobile application provides:

- Device discovery
- BLE connection
- Sensor monitoring
- Communication status
- Emergency notifications
- Device configuration
- Historical/event monitoring
- Future building-level emergency monitoring

The application is designed using Flutter so that the monitoring interface can be extended across supported mobile platforms.

## Project Status

The project is currently in the **prototype development and testing stage**.

The physical prototype demonstrates the integration of multiple sensors and output modules. Further work includes:

- ESP32-S3 integration
- Sensor calibration
- Controlled fire-risk testing
- Communication testing
- Mobile application integration
- Backend integration
- 4G/LTE and LoRa testing
- AI/ML-based anomaly detection
- Emergency routing and coordination

Quantitative performance values such as detection accuracy, response time, communication range, latency, and power consumption should only be reported after controlled experimental measurements.

## Future Scope

Future versions of IGNIS X can include:

- AI-based fire-risk prediction
- Sensor anomaly detection
- Multiple interconnected fire-monitoring nodes
- LoRa-based building-wide monitoring
- 4G/LTE communication failover
- Indoor localization
- Dynamic emergency route generation
- Firefighter/first-responder dashboards
- Cloud analytics
- Historical fire-risk analysis
- PCB and enclosure development

## Safety Disclaimer

IGNIS X is an academic prototype developed for research, learning, and demonstration purposes. It is **not a certified fire alarm, fire suppression system, or replacement for professionally approved life-safety equipment**.

All real-world deployment decisions should follow applicable safety standards, building regulations, professional engineering practices, and certified fire-protection requirements.

## Project

**Project Name:** IGNIS X  
**Full Name:** Intelligent Fire Intelligence System  
**Institution:** Woxsen University  
**Program:** B.Tech. Computer Science and Engineering – Artificial Intelligence and Machine Learning  
**Academic Year:** 2026–2027

---

### Building Safety. Powered by Intelligence.
