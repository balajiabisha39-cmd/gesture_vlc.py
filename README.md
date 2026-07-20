# gesture_vlc.py
A touchless media control system that enables users to control **VLC Media Player** using simple hand gestures. This project uses an **Arduino Uno** with **two HC-SR04 Ultrasonic Sensors** to detect hand movements and convert them into media control commands such as Play/Pause, Volume Control, Rewind, and Fast Forward.

---

# 📖 Project Overview

The Gesture Controlled VLC Media Player is an embedded systems project designed to provide a contactless and intuitive way of controlling multimedia playback. Instead of using a keyboard, mouse, or remote control, users interact with VLC Media Player through predefined hand gestures detected by ultrasonic sensors.

The system continuously measures the distance between the user's hands and the sensors. Based on these distance values, Arduino identifies specific gestures and sends commands to the computer, allowing VLC Media Player to perform different actions.

This project demonstrates the integration of **Arduino**, **Ultrasonic Sensors**, **Serial Communication**, and **Automation** to create an interactive Human-Computer Interface (HCI).

---

# 🎯 Objectives

- Develop a touch-free media control system.
- Control VLC Media Player using hand gestures.
- Demonstrate real-time gesture recognition.
- Improve user convenience through contactless interaction.
- Learn Arduino programming and serial communication.
- Explore embedded systems and human-computer interaction.

---

# ✨ Features

- 🎵 Play and Pause Media
- 🔊 Volume Up
- 🔉 Volume Down
- ⏩ Fast Forward
- ⏪ Rewind
- ✋ Gesture Lock Mechanism
- ⚡ Real-Time Gesture Detection
- 🖥️ Arduino-Based Implementation
- 📡 Contactless User Interface
- 💰 Low-Cost Hardware Design

---

# 🛠️ Hardware Components

- Arduino Uno
- 2 × HC-SR04 Ultrasonic Sensors
- USB Cable
- Jumper Wires
- Breadboard (Optional)
- Computer/Laptop

---

# 💻 Software Requirements

- Arduino IDE
- VLC Media Player
- Python 3.x
- PySerial Library
- Windows Operating System

---

# ⚙️ Working Principle

The system uses two ultrasonic sensors to monitor the position and movement of the user's hands.

- The **Left Sensor** is dedicated to **Volume Control**.
- The **Right Sensor** is dedicated to **Seek Control**.
- When **both sensors detect hands simultaneously**, VLC Media Player toggles between **Play** and **Pause**.

A lock gesture is used before executing Volume or Seek operations. Once a lock gesture is detected, moving the hand closer or farther from the sensor performs the corresponding media action.

---

# ✋ Gesture Controls

| Gesture | How to Perform | VLC Action |
|----------|----------------|------------|
| 👐 Both Hands Detected | Place both hands in front of both sensors (40–50 cm) | ▶️ Play / Pause |
| ✋ Left Lock Gesture | Hold left hand steady at 13–17 cm | 🔊 Enter Volume Control Mode |
| ⬆️ Left Push In | Move left hand closer than 10 cm | 🔊 Volume Up |
| ⬇️ Left Pull Out | Move left hand farther than 20 cm | 🔉 Volume Down |
| ✋ Right Lock Gesture | Hold right hand steady at 13–17 cm | ⏩ Enter Seek Control Mode |
| ➡️ Right Push In | Move right hand closer than 10 cm | ⏪ Rewind |
| ⬅️ Right Pull Out | Move right hand farther than 20 cm | ⏩ Fast Forward |

---

# 🔄 Workflow

1. Power on the Arduino and connect it to the computer.
2. Initialize both ultrasonic sensors.
3. Continuously measure the distance from both sensors.
4. Detect whether both hands are present.
5. If both hands are detected, execute **Play/Pause**.
6. If the left lock gesture is detected, activate **Volume Control Mode**.
7. Moving the left hand closer increases the volume.
8. Moving the left hand farther decreases the volume.
9. If the right lock gesture is detected, activate **Seek Control Mode**.
10. Moving the right hand closer rewinds the video.
11. Moving the right hand farther fast-forwards the video.
12. Repeat the process continuously for real-time gesture recognition.

---

# 📂 Project Structure

```
Gesture-Controlled-VLC-Player/
│
├── Arduino_Code/
│   └── gesture_control.ino
│
├── Python/
│   └── vlc_controller.py
│
├── Images/
│   ├── Circuit_Diagram.png
│   ├── Hardware_Setup.jpg
│   ├── Working.jpg
│   └── Output.jpg
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

# 🚀 Installation

## Clone the Repository

```bash
git clone https://github.com/yourusername/Gesture-Controlled-VLC-Player.git
```

## Navigate to the Project Folder

```bash
cd Gesture-Controlled-VLC-Player
```

## Install Required Python Library

```bash
pip install pyserial
```

## Upload Arduino Code

- Open Arduino IDE.
- Connect Arduino Uno.
- Select the correct Board and COM Port.
- Upload `gesture_control.ino`.

## Run the Python Program

```bash
python vlc_controller.py
```

---

# 📊 Applications

- Smart Home Automation
- Touchless Media Control
- Interactive Classrooms
- Healthcare Environments
- Public Display Systems
- Accessibility Solutions
- Smart Entertainment Systems

---

# 🎓 Learning Outcomes

Through this project, we gained practical experience in:

- Arduino Programming
- Embedded Systems
- Ultrasonic Sensor Interfacing
- Serial Communication
- Real-Time System Design
- Hardware and Software Integration
- Human-Computer Interaction (HCI)
- Automation Techniques
- Problem Solving
- Team Collaboration

---

# 🔮 Future Enhancements

- Camera-Based Gesture Recognition
- AI and Machine Learning Integration
- Bluetooth Connectivity
- Wi-Fi Based Media Control
- Voice and Gesture Hybrid Control
- Mobile Application Support
- Custom Gesture Configuration

---


# 👥 Team Members

- Balaji K
- Dhanavandhan SRS
- Arshanth Sree 3

---

# 🤝 Contributing

Contributions are welcome! Feel free to fork this repository, improve the project, and submit a pull request.

---

# 📜 License

This project is intended for educational and academic purposes.

---

# ⭐ Support

If you found this project useful, please consider giving this repository a **⭐ Star**. Your support is greatly appreciated!

---

## 📬 Contact

**Balaji K**  
Electronics and Communication Engineering (ECE)

📧 Email: balajiabisha39@gmail.com

🔗 LinkedIn: https://https://www.linkedin.com/in/balaji-k-70230533b?utm_source=share_via&utm_content=profile&utm_medium=member_android

💻 GitHub: https://github.com/balajiabisha39-cmd

---

**Made with ❤️ using Arduino and Embedded Systems**
