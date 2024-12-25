# ElevatorFaultDetection

The dataset utilized in this study was collected from advanced elevator monitoring and diagnostic systems deployed across high-rise commercial buildings in Tokyo, Japan. Spanning a period of nearly five years, from January 2020 to November 2024, the dataset contains hourly measurements recorded by a network of Internet of Things (IoT) sensors integrated into elevator systems. These sensors captured a diverse range of operational, mechanical, electrical, environmental, and maintenance-related parameters, making this dataset a comprehensive representation of real-world elevator operations.

The city of Tokyo was chosen for its extensive use of modern elevator technologies and stringent maintenance practices, ensuring the collection of high-quality, diverse data under varying operational scenarios. This includes data from residential apartments, office skyscrapers, and mixed-use buildings, providing a holistic view of elevator behavior under different load and environmental conditions. The dataset is inherently imbalanced, reflecting realistic distributions of normal operations and rare fault occurrences.

Features Overview
The dataset contains the following key features:

1. Core Operational Features
Motor Current (A): Current drawn by the elevator motor, indicating electrical load.
Motor Voltage (V): Voltage levels during operation, crucial for monitoring electrical stability.
Vibration Level (g): Measurements from accelerometers detecting mechanical vibrations.
Speed (m/s): Real-time speed of the elevator cabin during operation.
Cabin Position: Current floor or shaft position of the elevator.
2. Mechanical Features
Cabin Acceleration (m/s²): Acceleration rates of the cabin during motion.
Cabin Deceleration (m/s²): Deceleration rates of the cabin during stops.
Braking Force (N): Performance of the braking system under different loads.
Rope Tension (N): Tension levels in the elevator’s suspension ropes.
Guide Rail Condition Index: Quantitative measure of guide rail health.
Pulley Wear: Wear and tear levels in the elevator pulley system.
Lubrication Levels: Indication of lubrication sufficiency in mechanical components.
3. Electrical Features
Power Consumption (kWh): Energy usage of the elevator system.
Battery Health (%): Status of the backup power system.
Voltage Fluctuations (V): Deviations in the supplied voltage.
Current Harmonics: Irregularities in the electrical waveform.
4. Environmental Features
Ambient Temperature (°C): Environmental temperature near the elevator system.
Humidity (%): Humidity levels in the surrounding area.
Dust Levels (µg/m³): Concentration of dust and particulate matter.
External Vibration Levels (g): Vibrations caused by building movements or external factors.
5. Usage Features
Load (kg): Weight inside the elevator cabin during operation.
Passenger Count: Estimated number of passengers based on load sensors.
Number of Trips: Total trips performed by the elevator in a given period.
Stop Frequency: Number of stops per trip.
Travel Distance (m): Cumulative distance traveled over time.
Call Waiting Time (s): Time between a button press and elevator arrival.
6. Maintenance and Historical Features
Fault Logs: Historical records of fault occurrences.
Maintenance History: Logs of past repairs and servicing.
Component Age (Years): Age of critical elevator components like motors and brakes.
Last Serviced Days Ago: Days since the last maintenance activity.
MTTF (Mean Time to Failure): Estimated operational time between consecutive faults.
7. Advanced Diagnostic Features
Signal Noise: Variations in sensor signals indicative of irregularities.
Temperature Gradient (°C): Sudden changes indicating potential overheating.
Door Sensor Readings: Metrics to detect misalignments or obstructions.
Control System Delay (ms): Latency in responding to control commands.
Frequency of Emergency Stops: Instances where the elevator was stopped abruptly.
8. Predictive Features
RUL (Remaining Useful Life): Estimated cycles or time remaining before failure.
Health Indices: Composite scores for components like motors, brakes, and sensors.
9. Target Labels
Fault State (Binary Classification):
0: Normal operation.
1: Fault detected.
Fault Category (Multiclass Classification):
Categories: Door Failure, Motor Malfunction, Sensor Error, Brake Failure.
Fault Severity (Ordinal Classification):
Levels: Minor, Moderate, Critical.
Key Characteristics
Temporal Nature: Hourly timestamps allow temporal analysis and modeling of sequential patterns.
Imbalanced Data: Reflects real-world conditions where faults occur less frequently than normal operations.
Diversity of Features: Includes operational, environmental, and diagnostic metrics, making the dataset highly versatile for fault diagnosis tasks.
This dataset provides a robust foundation for developing intelligent fault diagnosis models and evaluating predictive maintenance strategies, offering significant potential for improving the safety, reliability, and efficiency of elevator systems.
