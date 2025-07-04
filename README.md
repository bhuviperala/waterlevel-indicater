# waterlevel-indicater

iot-water-level-indicator/
├── code/
│   ├── water_level_sensor.ino         # Arduino code
│   └── firebase_config.h              # Firebase credentials (use .gitignore)
├── circuit_diagram/
│   └── water_level_circuit.png        # Circuit diagram image
├── mobile_app/                        # Optional Flutter or MIT App
│   └── app_code_here
├── README.md
├── .gitignore
└── LICENSE


# 💧 IoT-Based Water Level Indicator

This project is a smart water level monitoring system using IoT. It uses an ultrasonic sensor to measure the water level in a tank and updates the data in real-time to Firebase. You can view the current water level on a mobile app or web dashboard.

---

## 🔧 Features

- Real-time water level monitoring
- Ultrasonic sensor (HC-SR04)
- NodeMCU (ESP8266) or ESP32
- Firebase integration
- Alerts for full/low water levels
- Mobile or web dashboard (optional)

---

## 📦 Components Required

| Component            | Quantity |
|----------------------|----------|
| ESP8266 (NodeMCU)    | 1        |
| Ultrasonic Sensor    | 1        |
| Jumper Wires         | 10+      |
| Breadboard           | 1        |
| Water Tank/Container | 1        |

---

## 🛠️ Circuit Diagram

![circuit](https://github.com/user-attachments/assets/65130c1c-9194-45e3-b685-9cb6487a5fdf)

![hardware tools](https://github.com/user-attachments/assets/f7bace66-e9f6-4f23-aaa3-ce2be9f90755)
![imaging](https://github.com/user-attachments/assets/ede2b1ec-d806-4c84-ac32-110c4c652819)
---

## 🧠 How It Works

1. The HC-SR04 sensor calculates the distance between itself and the water surface.
2. NodeMCU reads the distance and converts it into a water level percentage.
3. Data is sent to Firebase.
4. A mobile/web app retrieves the data and displays it in a user-friendly format.
5. Alerts can be triggered for specific levels (optional).
