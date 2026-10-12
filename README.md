# Arduino Firefighting Robot

An Arduino-based IoT robot that detects fire using a flame sensor and automatically switches on a water pump to put it out.

## Features
- Detects flame using a flame sensor module
- Automatically turns on a water pump through a relay
- Buzzer / LED alert while fire is detected (optional)
- Simple, low-cost, and easy to extend (motors, Wi-Fi alerts, etc.)

## Components Used
| Component | Quantity |
|-----------|----------|
| Arduino Uno / Nano | 1 |
| Flame sensor module | 1 |
| Relay module (5V) | 1 |
| Mini water pump | 1 |
| Battery / power supply | 1 |
| Jumper wires, breadboard | as needed |

## How It Works
1. The flame sensor continuously monitors for infrared light from a flame.
2. When fire is detected, the Arduino reads the sensor output.
3. The Arduino triggers the relay, which powers the water pump.
4. When the flame is gone, the pump switches off.

## Pin Connections
| Arduino Pin | Connected To |
|-------------|--------------|
| D2 | Flame sensor (DO) |
| D7 | Relay IN |
| D8 | Buzzer (optional) |
| 5V / GND | Sensor and relay power |

> Update this table to match your actual wiring.

## Circuit Diagram
Add your circuit diagram or photo in `docs/` and link it here:

`![Circuit](docs/circuit.png)`

## Getting Started
1. Clone the repo:
   ```
   git clone https://github.com/jayatkarne/arduino-firefighting-robot.git
   ```
2. Open `src/firefighting_robot.ino` in the Arduino IDE.
3. Select your board and port, then upload.
4. Power the circuit and test with a lighter flame at a safe distance.

## Demo
Add a photo or video link here.

## Future Improvements
- Add wheels/motors for a moving robot
- Send alerts to phone using ESP8266/ESP32
- Add a smoke sensor (MQ-2) for early detection

## What I Learned
Arduino programming in embedded C, sensor interfacing, relay control, and IoT basics, built during my robotics internship at DoxPro Robotics.

## Author
**Jay Atkarne**
GitHub: [jayatkarne](https://github.com/jayatkarne)
Email: jayatkarne@gmail.com
