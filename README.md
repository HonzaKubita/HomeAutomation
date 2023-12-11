# Home Automation Project

Welcome to the Home Automation Project, a versatile and modular system designed to automate your room. This project allows you to control lighting, regulate temperature, open and close window blinds, and more. The architecture is designed for modularity, empowering users to create their own modules and expand the capabilities of their home automation setup.

## System Overview

### Software

#### Hub
The central control unit is a Raspberry Pi equipped with a touch screen, serving as the main interface through a Control Panel web application. The Control Panel interacts with a Flask backend running on the Raspberry Pi, which, in turn, communicates with the modules.

The Flask server on the Raspberry Pi is responsible for controlling the GPIO (General Purpose Input/Output) to manage various functionalities within the system.

#### Modules
Each module in the system is based on an ESP8266 running MicroPython. The main firmware, provided by this project, serves as a foundation, and additional extensions can be built on top to support different types of modules.

### Hardware

#### Hub
The hub hardware consists of a Raspberry Pi connected to a custom board featuring multiple RJ-45 connectors. These connectors facilitate communication and power delivery to connected modules. Although the connectors use a proprietary protocol, they provide a versatile way to attach any module to any connector on the hub. CAT6 Ethernet cables are used for connection.

#### Modules
Every module contains an ESP8266 responsible for communication with the hub. The ESP8266 serves as a foundation, allowing users to build custom functionalities on top. For example, a module could control a servo for a radiator regulator or incorporate a relay to manage a light switch.

## Contributing

I encourage contributions to make this home automation platform even more powerful and versatile. Feel free to submit issues, feature requests, or pull requests on this GitHub repository.
