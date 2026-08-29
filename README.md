# Self Balancing Robot

A two-wheeled, self-balancing robot built using an Arduino Nano, MPU-6050, and L298N motor driver. This project utilizes Proportional-Integral-Derivative (PID) control algorithms to maintain equilibrium[cite: 1].

This project was developed as a Major Project for the Bachelor of Technology in Electronics & Communication Engineering at Gyan Ganga Institute of Technology & Science[cite: 1].

 👥 Team
* Ashwani Rai (0206EC201012)[cite: 1]
* Ayushi Shukla (0206EC201014)[cite: 1]
* Manas Tiwari (0206EC201025)[cite: 1]
* Shrubhi Yadav (0206EC201051)[cite: 1]

**Under the guidance of:** Prof. Shailesh Khaparker[cite: 1]

## 🛠️ Hardware Requirements
To build this robot, you will need the following components:

| Component | Quantity | Role |
| :--- | :--- | :--- |
| **Arduino Nano** | 1 | The central controller for processing sensor data and controlling motors[cite: 1]. |
| **MPU-6050** | 1 | IMU sensor for measuring acceleration and gyroscopic data to determine orientation[cite: 1]. |
| **L298N Motor Driver** | 1 | Controls the speed and direction of the motors[cite: 1]. |
| **BO Motors** | 2 | Brushed DC motors for propulsion and balance control[cite: 1]. |
| **BO Wheels** | 2 | Provide mobility and traction[cite: 1]. |
| **Sun Board** | 3 | Used for the lightweight and sturdy chassis[cite: 1]. |
| **Battery Holder** | 1 | Secures the power source[cite: 1]. |
| **Breadboard & Jumpers**| 1 | For prototyping and electrical connections[cite: 1]. |
| **9V Batteries** | 2 | Provide power for the motor and circuit separately[cite: 1]. |

*(Total estimated cost: Rs. 1160.00)*[cite: 1]

## 💻 Software Requirements
* **Operating System:** Windows 11[cite: 1]
* **Software:** Arduino IDE[cite: 1]
* **Required Libraries:**
  * `PID_v1`[cite: 1]
  * `LMotorController`[cite: 1]
  * `I2Cdev`[cite: 1]
  * `MPU6050_6Axis_MotionApps20`[cite: 1]
  * `Wire`[cite: 1]

## ⚙️ How It Works
The robot operates as an inverted pendulum[cite: 1]. The MPU-6050 measures the robot's tilt angle and angular velocity in real-time[cite: 1]. This data is processed by the Arduino Nano using a PID controller, which calculates the deviation from the upright position[cite: 1]. The Arduino then sends signals to the L298N motor driver to adjust the speed and direction of the BO motors, counteracting the tilt and keeping the robot balanced[cite: 1]. 

### Tuning the PID
Balancing requires finding the correct Proportional (P), Integral (I), and Derivative (D) values[cite: 1].
1. Set `Ki` and `Kd` to 0.[cite: 1]
2. Adjust `Kp` until the robot can briefly balance but oscillates[cite: 1].
3. Adjust `Kd` to minimize oscillations[cite: 1].
4. Adjust `Ki` as needed for fine-tuning[cite: 1].

## 🚀 Setup & Installation
1. Assemble the hardware components onto the Sun Board chassis[cite: 1].
2. Connect the components according to the circuit diagram[cite: 1]. *Note: Use separate power sources for the motors and the circuit for isolation. Remove the jumper on the L298N module if using a supply voltage greater than 12V[cite: 1].*
3. Install the Arduino IDE and the required libraries[cite: 1].
4. Open `SelfBalancingRobot.ino` in the Arduino IDE[cite: 1].
5. Upload the code to the Arduino Nano[cite: 1].
6. Hold the robot upright while the MPU-6050 calibrates[cite: 1].

## 🔮 Future Scope
Future enhancements could include:
* Obstacle detection and avoidance[cite: 1].
* Wireless control via Bluetooth or Wi-Fi[cite: 1].
* Integration of computer vision for navigation[cite: 1].
* AI and machine learning for adaptive stability[cite: 1].
