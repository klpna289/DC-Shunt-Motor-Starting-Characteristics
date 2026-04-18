# DC Shunt Motor Starting Characteristics (MATLAB/Simulink)

## Objective
To study and simulate the starting characteristics of a DC shunt motor using step-wise resistance control in MATLAB/Simulink.

## Tools Used
- MATLAB
- Simulink (Simscape Electrical)

## Description
This project models a DC shunt motor and analyzes its starting behavior using a step-by-step resistance control method.

At the time of starting, the back EMF is zero, which causes a very high armature current. To protect the motor, external resistances are connected in series with the armature circuit. These resistances are gradually removed using controlled switching.

In this simulation, multiple breakers (switches) are used along with step inputs to remove resistances sequentially, allowing smooth acceleration of the motor.

## Simulation Model
- Step blocks are used to control switching at different time intervals  
- Breakers act as switches to remove resistances step-by-step  
- Resistances (R1–R5) limit starting current  
- DC machine block represents the shunt motor  
- Powergui is set to continuous mode  

## Components Used
- DC Voltage Source (Armature supply)
- DC Voltage Source (Field supply)
- DC Shunt Motor (DC Machine block)
- Starting Resistances (R1–R5)
- Breakers (controlled switches)
- Step Input Blocks (Step1–Step6)
- Voltage Measurement Block
- Bus Selector
- Scope
- XY Graphs (for characteristic curves)

## Outputs Observed
- Speed (ω)
- Electromagnetic Torque (Te)
- Armature Current (Ia)
- Field Current (If)

## Results
- High armature current is observed at starting  
- Step-by-step removal of resistance reduces current gradually  
- Motor speed increases smoothly with time  
- Torque varies during the starting process  
- Graphs show relationship between speed, torque, and current  

## Learning Outcome
- Understood practical starting method of DC shunt motor  
- Learned step control using breakers in Simulink  
- Analyzed dynamic performance (speed, torque, current)  
- Gained hands-on experience with Simscape Electrical components  

## Author
Kalpna Painkra
