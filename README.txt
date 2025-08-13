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

MATLAB Version
Tested in MATLAB R2024
