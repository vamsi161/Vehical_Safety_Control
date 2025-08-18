# Multi-Sensor Vehicle Safety Control – Current Build


Multi-Sensor Vehicle Safety Control – Current Build

This MATLAB/Simulink project models a simplified vehicle safety system that integrates environmental and vehicle dynamics sensing with decision-making logic to enhance safety under adverse conditions.

Overview
The system consists of:

Sensing Stage

Simulates rain intensity with realistic profiles and noise.

Generates wheel speed signals from a base speed source with optional noise.

Simulates steering angle variations with optional noise. These signals emulate real sensor outputs and provide input to the safety logic.

Safety Manager Stage

Monitors the sensor inputs in real time.

Evaluates driving conditions and potential risks.

Issues control signals to adjust vehicle behavior such as reducing speed in heavy rain or during sharp steering.

Current Status

All sensor subsystems implemented and tested.

Safety Manager block integrated with sensor outputs.

Output signals validated through simulation plots.

Next Steps

Connect the control signals to a vehicle dynamics plant model for co-simulation.

Tune thresholds and control logic for different driving scenarios.

Create polished documentation and visuals for portfolio presentation.

Update: 18-08-2025

Status: functional end-to-end, controller overshoot under step changes. refining model need to be done.


Current Functionality:
- Sensor Subsystem: rain intensity, wheel speed, and steering angle simulation with noise injection.
![Sensor Outputs](https://github.com/vamsi161/Vehical_Safety_Control/blob/main/scope_outputs/Sensor_outputs.png)
- Safety Manager: computes a maximum safe vehicle speed based on conditions.
- Speed Governor: enforces the lower of driver command or safe limit.
- PI Controller + Plant: basic vehicle speed response simulation.

Known Issues:
- Overshoot present in the PI response.

Next Steps:
- Refine controller to reduce overshoot.





MATLAB Version
Tested in MATLAB R2024
