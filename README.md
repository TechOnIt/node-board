# node-board
Manages IoT devices at the edge. Reads sensor data, executes relay commands, and communicates with the master board in a distributed IoT setup.


## Features
- Reads data from sensors (temperature, humidity, light, etc.)
- Controls relays and actuators
- Maintains offline operation and caches data
- Receives automation commands from Controller

## Architecture
- **Node Devices**: Collect sensor data, execute commands, provide local safety.
- **Controller Node**: Aggregates Node data, communicates with cloud, caches automation rules.
- See also:
  - [agent-controller](https://github.com/your-org/agent-controller)
  - [agent-sdk](https://github.com/your-org/agent-sdk)

## Technologies
- MicroPython for ESP32 / NodeMCU
- Python 3 for Controller
- MQTT, Wi-Fi
- PlatformIO for building Node firmware

## Getting Started
1. Connect Node to Wi-Fi network
2. Configure Node with `nodeId` and Controller endpoint
3. Start Node to begin sending sensor data and receiving commands

## Goal
Provide a modular, scalable, and testable edge layer for IoT automation.
