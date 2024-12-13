# Cost Effective Smart Home Management Solutions

This project provides a smart home management solution that enables users to control home appliances via the Blynk IoT platform. The system integrates sensors and relays to manage devices like lights, fans, and other home appliances. It also monitors environmental parameters like temperature, humidity, and water levels.

## Table of Contents

- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Remote Control**: Control up to four home appliances remotely via the Blynk app.
- **Environmental Monitoring**: Monitor temperature, humidity, and water levels in real time.
- **Manual Control**: Option to manually control devices using physical switches.
- **Customizable**: Easily extend the system to support more devices and sensors.

## Hardware Requirements

- ESP32/NodeMCU
- Relays (4-channel)
- DHT11 Temperature and Humidity Sensor
- Ultrasonic Sensor (HC-SR04) for water level monitoring
- Jumper wires
- Power supply (5V)

## Software Requirements

- Arduino IDE
- Blynk Library
- Blynk App (Android/iOS)

## Setup and Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ChaitanyaNarang28/Cost-effective-smart-home-management-solutions.git
   cd Cost-effective-smart-home-management-solutions
   ```

2. **Install the Required Libraries**:
   - Open Arduino IDE.
   - Go to `Sketch` > `Include Library` > `Manage Libraries`.
   - Search for `Blynk` and install it.
   - Install the `DHT sensor library`.

3. **Configure Blynk**:
   - Replace the `BLYNK_AUTH_TOKEN` in the code with your own Blynk token.
   - Update the WiFi credentials in the `BlynkEdgent.h` file.

4. **Upload the Code**:
   - Connect your ESP32/NodeMCU to your computer.
   - Select the correct board and port in Arduino IDE.
   - Upload the code to the board.

## Usage

- **Blynk App**:
  - Open the Blynk app on your smartphone.
  - Add buttons linked to the virtual pins `V1` to `V4` to control the relays.
  - Monitor temperature and humidity on virtual pins `V7` and `V8`.
  - Monitor water level on virtual pin `V5`.

- **Manual Control**:
  - Use the physical switches connected to the GPIO pins to control the appliances manually.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
