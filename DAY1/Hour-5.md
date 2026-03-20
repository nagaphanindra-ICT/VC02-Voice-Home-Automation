# Day 1 – Hour 5 (2:00 AM – 3:00 AM)

## Objective
To enhance the system by implementing fan speed control and validating the design using simulation.

## Work Done
- Implemented fan speed control using capacitive dimming technique
- Simulated the fan control circuit using simulator
- Observed waveform changes for different capacitor values
- Verified different speed levels based on capacitance
- Attached simulation screenshots as proof

## Additional Work
- Studied working of traditional fan regulators
- Reverse engineered an old fan regulator circuit
- Designed similar capacitive control circuit for the project

## Key Feature
- Unlike basic home automation systems (only ON/OFF control), this system supports fan speed control using voice commands
- Enables multiple speed levels using relay-based capacitor switching

## Technical Understanding
- Capacitors control current flow in AC circuits
- Different capacitor values produce different fan speeds
- Relay switches between capacitors based on GPIO signals

## Simulation Results
- 2.2µF capacitor → Low speed
- 3.3µF capacitor → Medium speed
- Combined capacitors → High speed

## Learning
- Practical understanding of AC fan speed control
- Integration of electronics and embedded systems
- Importance of simulation before real implementation

## Simulation Proof
![Simulation 1](../fan_simulation_1.png)
![Simulation 2](../fan_simulation_2.png)
![Simulation 3](../fan_simulation_3.png)
