

---

# Accident Detection and Prevention System using IoT and Machine Learning

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [Setup and Installation](#setup-and-installation)
- [How It Works](#how-it-works)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project enhances road safety in **hairpin curves** and **hilly areas** using **IoT (Internet of Things)** and **Machine Learning (ML)** technologies. It focuses on **preventing accidents** and providing **real-time alerts** to drivers. Using **YOLO (You Only Look Once)** object detection, the system detects approaching vehicles, warns drivers about hazards, and sends alerts to emergency responders in case of accidents.

## Features
- **Real-time Vehicle Detection**: YOLO detects vehicles approaching dangerous curves.
- **Driver Alerts**: Notifies drivers with **LED indicators**, **buzzers**, and a **16x2 display**.
- **Accident Detection and Notification**: Sends automatic alerts to responders via **GSM** and **GPS**.
- **IoT Integration**: **NodeMCU (ESP8266)** manages communication between devices.

## Technologies Used
- **YOLO**: Object detection algorithm trained on **COCO** dataset.
- **ESP32 Camera Module**: Captures live video for detection.
- **NodeMCU (ESP8266)**: Handles IoT communication.
- **GSM & GPS Modules**: Sends accident notifications and provides location tracking.
- **Firebase**: Stores detection and accident data.

## System Architecture
1. **ESP32 Camera Module**: Captures real-time video of the road.
2. **YOLO**: Detects vehicles approaching hairpin curves.
3. **NodeMCU**: Triggers alerts via **LED**, **buzzer**, and **16x2 display**.
4. **GSM & GPS**: Sends emergency notifications with location.

## Setup and Installation
### Hardware Requirements:
- ESP32 Camera, NodeMCU (ESP8266), GSM & GPS modules, LED, Buzzer, 16x2 Display.

### Software Requirements:
- Python (for YOLO), OpenCV, TensorFlow, Arduino IDE, Firebase account.

### Installation Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/accident-detection-prevention.git
   cd accident-detection-prevention
   ```
2. Set up YOLO with the required libraries:
   ```bash
   pip install opencv-python tensorflow keras
   ```
3. Upload code to ESP32 and NodeMCU using Arduino IDE.
4. Configure GSM & GPS modules for sending notifications.

## How It Works
1. **Detection**: ESP32 captures video, YOLO detects vehicles.
2. **Alerts**: LED lights, buzzers, and display warn drivers.
3. **Accident Response**: GSM sends notifications, GPS shares location.
4. **Data Storage**: Detection and accident data stored in Firebase.

## Future Enhancements
- Integrate **weather sensors** to monitor road conditions.
- Add **voice alerts** or mobile notifications for drivers.
- Extend system to monitor **other hazards** like landslides.

## Contributing
1. Fork the repo, create a new branch, make changes, and submit a pull request.

## License
Licensed under the MIT License – see [LICENSE](LICENSE) for details.

---


