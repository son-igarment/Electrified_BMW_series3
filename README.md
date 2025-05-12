# Electrified BMW Series 3 Simulation Model

## Owner
Phạm Lê Ngọc Sơn

## Project Overview
This project contains a MATLAB/Simulink-based simulation model for an electrified BMW Series 3 vehicle. The model allows for the analysis of vehicle performance, power consumption, and efficiency under various driving conditions.

## Project Structure
- `vehicle_model.slx` - Main Simulink model of the electrified vehicle
- `STARTER.m` - Main script to initialize and run simulations
- `DATI_Veicolo.m` - Vehicle parameters and characteristics (mass, aerodynamics, etc.)
- `brushless_motor_characteristic.m` - Motor performance characteristics
- `internal_permanent_magnet_motor.m` - Motor specifications
- `cycles_wltp.mat` - WLTP driving cycle data
- `PROF_Artemis_Bologna_Roma.mat` - Artemis driving cycle data for Bologna-Roma route
- `ZAP.m` - Utility script

## Features
- Detailed vehicle dynamics simulation
- Electric motor performance analysis
- Power consumption calculations 
- Driving cycle simulations
- Efficiency analysis at different speeds and loads

## Usage Instructions

### Prerequisites
- MATLAB (R2019b or later recommended)
- Simulink
- Control System Toolbox
- Simscape (for advanced physical modeling)

### Getting Started
1. Open MATLAB and navigate to the project directory
2. Run the `STARTER.m` script to initialize all parameters:
   ```matlab
   STARTER
   ```
3. This script will:
   - Load motor characteristics
   - Set vehicle parameters
   - Load driving cycles

### Running Simulations
1. After initialization, open the `vehicle_model.slx` file:
   ```matlab
   open('vehicle_model.slx')
   ```
2. Set simulation parameters in the Simulink model
3. Run the simulation to analyze vehicle performance

### Analyzing Results
- The model outputs various performance metrics:
  - Vehicle speed and acceleration
  - Motor torque and power
  - Energy consumption
  - System efficiency

## Vehicle Parameters
The model is configured for a BMW Series 3 with the following default specifications:
- Curb weight: 1342 kg (without batteries)
- Battery weight: 350 kg
- Aerodynamic drag coefficient × frontal area: 0.652
- Wheel size: 205/60 R16
- Gear ratio: 4.3

## Customization
You can modify vehicle parameters in `DATI_Veicolo.m` or adjust motor characteristics in `internal_permanent_magnet_motor.m` to simulate different vehicle configurations.