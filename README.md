# Arduino-Line-Following-Robot
Arduino UNO based four-wheel autonomous line-following robot using IR sensors and L298N motor driver.
# Arduino UNO Based Four-Wheel Line Following Robot 🚗

An autonomous four-wheel robot car built using Arduino UNO, infrared (IR) sensors and an L298N motor driver. The robot detects and follows a black line on a white surface without manual control.

## 📌 Project Overview

This project demonstrates the development of an autonomous line-following robot using embedded systems and sensor-based decision-making.

Two IR sensors detect the black line and send digital signals to the Arduino UNO. Based on the sensor readings, the Arduino controls the four DC gear motors through the L298N motor driver.

## 🎯 Objectives

- Build an autonomous four-wheel line-following robot.
- Interface IR sensors with Arduino UNO.
- Control motor direction and speed using an L298N motor driver.
- Understand sensor-based decision-making and embedded systems.

## 🛠️ Components Used

| Component | Quantity |
|---|---:|
| Arduino UNO R3 | 1 |
| L298N Motor Driver | 1 |
| IR Sensor Modules (LM393) | 2 |
| Yellow TT DC Gear Motors | 4 |
| Robot Chassis and Wheels | 1 set |
| 18650 Rechargeable Batteries | 2 |
| Jumper Wires | As required |
| Black Insulation Tape | As required |

## 🔌 Pin Connections

### IR Sensors to Arduino UNO

| IR Sensor | Arduino Pin |
|---|---|
| Left Sensor OUT | D2 |
| Right Sensor OUT | D3 |
| Both Sensors VCC | 5V |
| Both Sensors GND | GND |

### L298N Motor Driver to Arduino UNO

| L298N Pin | Arduino Pin |
|---|---|
| ENA | D11 |
| IN1 | D10 |
| IN2 | D9 |
| IN3 | D8 |
| IN4 | D7 |
| ENB | D6 |
| GND | Arduino GND |

### Motors to L298N

- OUT1 and OUT2: Two left-side motors connected in parallel.
- OUT3 and OUT4: Two right-side motors connected in parallel.

### Power Supply

- Battery supply connects to the L298N motor power input.
- Arduino and L298N share a common GND.
- IR sensors receive regulated 5V power from the Arduino UNO.

## ⚙️ Working Principle

1. IR sensors detect the surface using reflected infrared light.
2. The sensors send digital signals to Arduino UNO.
3. Arduino processes the sensor readings.
4. The L298N motor driver controls the direction and speed of the motors.
5. The robot moves forward, turns left, turns right or stops according to the sensor readings.

### Sensor Decision Logic

| Left Sensor | Right Sensor | Robot Action |
|---|---|---|
| LOW | LOW | Move Forward |
| LOW | HIGH | Turn Right |
| HIGH | LOW | Turn Left |
| HIGH | HIGH | Stop |

## 💻 Software Used

- Arduino IDE
- Embedded C/C++
- Arduino UNO
- Serial Monitor for sensor testing

## 🚀 How to Run the Project

1. Install Arduino IDE.
2. Connect Arduino UNO to your computer using USB.
3. Open `LineFollowingRobot.ino`.
4. Select Board: Arduino UNO.
5. Select the correct COM port.
6. Upload the program.
7. Connect the motor driver and verified power supply.
8. Place the robot on a black line over a white surface.

## ✨ Features

- Autonomous line detection.
- Four-wheel drive mechanism.
- Real-time IR sensor readings.
- Motor direction and speed control.
- Low-cost educational robotics project.

## 🔮 Future Improvements

- Implement PID control for smoother movement.
- Add ultrasonic obstacle detection.
- Add Bluetooth or Wi-Fi connectivity.
- Improve turning accuracy using additional IR sensors.

## 👨‍💻 Project Team

**Third Year – Artificial Intelligence & Data Science**

- Pranav Ubale
- Gaurav Suryavanshi
- Prathamesh Sonawane
- Pavan Shinde

**Academic Year:** 2026–27

## 📄 Project Documentation

Refer to `IoT_Mini_Project_Line_Following_Robot.pdf` in this repository for the detailed project report, circuit diagram, connections, Arduino code and testing results.

## 📜 License

This project is available for educational and learning purposes.
