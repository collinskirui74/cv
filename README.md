# MATLAB Simulation Files
# IoT Based Car Parking and Online Reservation System
# Author: Collins Kipngetich Kirui
# Institution: Technical University of Mombasa

## Overview

This directory contains MATLAB simulation files for the IoT-based Car Parking and Online Reservation System. These simulations are designed to verify the functionality of the proposed system before hardware implementation.

## Files Description

### 1. parking_simulation_main.m
Main simulation script that simulates the entire parking system operation.
- Simulates 5 parking slots
- Random car arrivals and departures
- QR code validation process
- Real-time slot availability updates
- Visualization of results

**To Run:** Open in MATLAB and run

### 2. system_architecture_diagram.m
Creates a visual block diagram showing:
- Application Layer (User Interface)
- Network Layer (Cloud/Firebase)
- Physical Layer (Hardware Components)
- Communication flow between layers

**To Run:** Open in MATLAB and run. Diagram will be saved as PNG.

### 3. system_flowchart.m
Creates a detailed flowchart of the system operation:
- User booking process
- Vehicle arrival detection
- QR code authentication
- Barrier control
- Slot monitoring

**To Run:** Open in MATLAB and run. Flowchart will be saved as PNG.

### 4. ir_sensor_simulation.m
Simulates IR sensor operation for parking slot detection:
- 5 IR sensors monitoring individual slots
- Vehicle presence detection
- Available slot counting
- Occupancy statistics

**To Run:** Open in MATLAB and run.

### 5. ultrasonic_sensor_simulation.m
Simulates HC-SR04 ultrasonic sensors at entry/exit gates:
- Vehicle distance measurement
- Echo pulse width calculation
- Gate trigger detection
- Timing analysis

**To Run:** Open in MATLAB and run.

### 6. servo_motor_control.m
Simulates servo motor operation for barrier control:
- PWM signal generation for different angles
- Barrier open/close timing
- Motor control logic

**To Run:** Open in MATLAB and run.

### 7. qr_code_authentication.m
Simulates QR code authentication process:
- QR code data structure
- Validation flow
- Test cases for valid/invalid codes

**To Run:** Open in MATLAB and run.

### 8. esp32_firebase_integration.m
Simulates ESP32 communication with Firebase:
- Wi-Fi data transmission
- JSON data structure
- Network latency analysis
- Connection status monitoring

**To Run:** Open in MATLAB and run.

### 9. hardware_circuit_diagram.m
Creates a complete hardware circuit diagram showing:
- Power supply connections
- ESP32 pin configuration
- Sensor connections (IR, Ultrasonic)
- Actuator connections (Servo motors)
- LCD display interface
- LED indicators

**To Run:** Open in MATLAB and run. Diagram will be saved as PNG.

## System Components Summary

| Component | Model | Quantity | Purpose |
|-----------|-------|----------|---------|
| Microcontroller | ESP32 | 1 | Main controller |
| Camera/QR Scanner | ESP32-CAM | 1 | QR code scanning |
| IR Sensors | Generic | 5 | Slot detection |
| Ultrasonic Sensors | HC-SR04 | 2 | Gate detection |
| Servo Motors | MG996R | 2 | Barrier control |
| LCD Display | 16x2 I2C | 1 | Local status |
| LEDs | 5mm | 5 | Status indicators |

## How to Use

1. Ensure MATLAB is installed with Image Processing Toolbox
2. Navigate to this directory in MATLAB
3. Run individual simulation files as needed
4. Generated PNG diagrams will be saved in this directory
5. Modify parameters in each file to match your requirements

## Simulation Parameters

- Number of Parking Slots: 5
- Simulation Time: 60 seconds (configurable)
- Arrival Rate: 0.1 cars/second (configurable)
- Departure Rate: 0.05 cars/second (configurable)
- Firebase Update Interval: 5 seconds
- Barrier Open Time: 2 seconds
- QR Validation Timeout: 3 seconds

## Expected Outputs

- Real-time parking slot status graphs
- System architecture diagrams
- Flowcharts for system operation
- Sensor response visualizations
- Network communication analysis
- Hardware circuit diagrams

## Notes

- These simulations are for verification purposes
- Hardware implementation may require modifications
- Ensure proper safety measures during hardware testing
- Follow manufacturer specifications for all components
