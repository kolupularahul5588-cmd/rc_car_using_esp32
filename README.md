**🚗 RC Car
📌 Project Description**

The RC Car is a Wi-Fi controlled 4WD robotic vehicle built using an ESP32 microcontroller and an L298N motor driver.
The system creates its own wireless network and hosts a web-based control panel, allowing users to drive the car and perform multiple stunt actions directly from any smartphone, tablet, or computer browser without requiring a dedicated mobile application.

This project demonstrates the integration of embedded systems, wireless networking, and robotics control to create an interactive and responsive robotic platform.

**🎯 Features**

📶 ESP32 SoftAP (no internet required)
🌐 Web-based control interface
🎮 Real-time drive controls (Forward, Backward, Left, Right, Stop)
🎪 12 pre-programmed stunt modes
⏱️ Auto-stop safety timer
🌗 Light & Dark mode UI
📊 Live status feedback
📱 Fully responsive design (mobile friendly)

**🧰 Hardware Requirement**s

ESP32 Development Board
L298N Motor Driver Module
4 DC Gear Motors
4WD Robot Chassis
Li-ion / LiPo Battery Pack
Connecting wires

**🔌 Pin Connections**
| **Component**         | **ESP32 Pin** | **L298N Pin** | **Purpose**                             |
| --------------------- | ------------- | ------------- | --------------------------------------- |
| Left Motor Direction  | GPIO 27       | IN1           | Controls left motor direction           |
| Left Motor Direction  | GPIO 26       | IN2           | Controls left motor direction           |
| Right Motor Direction | GPIO 25       | IN3           | Controls right motor direction          |
| Right Motor Direction | GPIO 33       | IN4           | Controls right motor direction          |
| Left Motor Enable     | GPIO 14       | ENA           | Enables / speed control for left motor  |
| Right Motor Enable    | GPIO 12       | ENB           | Enables / speed control for right motor |
| Ground                | GND           | GND           | Common ground reference                 |

⚠️ Ensure ESP32 GND and L298N GND are connected together.

| **Source**          | **Connect To** | **Purpose**                        |
| ------------------- | -------------- | ---------------------------------- |
| Battery +V          | L298N 12V      | Motor power supply                 |
| Battery GND         | L298N GND      | Power ground                       |
| L298N 5V (optional) | ESP32 VIN      | Power ESP32 (if regulator enabled) |


**💻 Software & Technologies**

Arduino IDE
ESP32 WiFi Library
WebServer Library
HTML, CSS, JavaScript (embedded UI)

**⚙️ Working Principle**

The ESP32 initializes in Access Point mode and creates a Wi-Fi network.

A built-in web server hosts a control dashboard.

User commands from the browser are sent as HTTP requests.

The ESP32 processes these requests and controls motor directions via the L298N driver.

Stunt functions execute predefined motion sequences for dynamic movements.

**🎪 Stunt Modes**

Tank Spin
Crab Walk
Drift Circle
Power Slide
Helicopter Spin
Snake Dance
Moonwalk
Donut
Bounce
4WD Crawl
Figure 8
Victory Dance

**🛡️ Safety Feature
**
Drive commands automatically stop after 5 seconds to prevent unintended continuous motion.

**🚀 How to Use**

Upload the code to ESP32 using Arduino IDE

Power the robot

Connect to Wi-Fi network:

SSID: ESP32_CAR
Password: 12345678

Open browser and go to: http://192.168.4.1

Use the control panel to drive and perform stunts

**📚 Learning Outcomes**

ESP32 Wi-Fi programming
Embedded web server development
Motor driver interfacing
Robotics motion control
IoT user interface design
**
🔮 Future Improvements**

Speed control using PWM
Joystick control mode
Camera streaming (ESP32-CAM)
Mobile app integration
Obstacle avoidance

**👨‍💻 Author**

Kolupula Rahul
Electronics & Communication Engineering
