# AeroPath 🚁

A Python-based drone fleet logistics and navigation system designed to manage drone movement, packages, pathfinding, flight constraints, and real-time simulation without using external databases.

## 🎯 Project Objective

AeroPath provides a complete system for managing a fleet of drones and coordinating their missions on a grid-based map.

The system can:
- Manage drones and packages.
- Save and load fleet data using JSON files.
- Find paths while avoiding no-fly zones.
- Calculate flight constraints based on gravity and payload mass.
- Simulate drone movement in real time.
- Monitor battery levels and automatically handle low-battery situations.
- Visualize the fleet and map using Matplotlib.

## ✨ Features

### 1. Data Structures
- `Drone` class for managing drone information and missions.
- `Package` class for managing package information.
- `Fleet` class for managing multiple drones and packages.
- JSON-based persistence to save and load the fleet state.

### 2. Pathfinding
- Grid-based pathfinding algorithm.
- Support for registering no-fly zones.
- Collision and coordinate validation.

### 3. Mission Logic
- Flight Envelope calculation.
- Considers:
  - Gravity
  - Payload mass
  - Battery level
- Checks whether a drone has enough battery to complete a mission.

### 4. Real-Time Simulation
- Simulates drone movement on the grid.
- Displays drone movement using Matplotlib.
- Monitors battery level during the mission.
- When battery reaches 10%, the drone cancels its mission and returns to `(0,0)`.

### 5. Command-Line Interface (CLI)
The main interface allows the user to:

- Add/Register new drones.
- Add/Register packages.
- Set no-fly zones.
- Start the flight simulation.
- Display the "Champions of Efficiency" based on log files.


