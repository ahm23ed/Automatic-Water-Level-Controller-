# Automatic-Water-Level-Controller-
The Automatic Water Level Controller is a PLC-based system designed to maintain the water level in a tank. The system uses water level sensors to control a pump, ensuring the water level remains within the desired range. This project aims to prevent overflow and dry running of the pump, thereby improving operational efficiency and conserving water.
----------------------------------------------------------------------------------------------------------------
Technologies Used
----------------------------------------------------------------------------------------------------------------
PLC: Siemens S7-1200 (or any other PLC)
Ladder Logic
Water level sensors (Low-Level Sensor and High-Level Sensor)
Relay and pump control
Optional: HMI for real-time monitoring and manual control
Components
PLC: Siemens S7-1200
Sensors: Two water level sensors (Low-Level Sensor and High-Level Sensor)
Actuator: Water pump controlled via relay
Power Supply: For the PLC and pump
HMI (optional): For real-time monitoring and manual control
Operation Logic
Inputs:

I0.0: Low-Level Sensor (LLS)
I0.1: High-Level Sensor (HLS)
Outputs:

Q0.0: Pump Control Relay
Logic:

When the water level falls below the Low-Level Sensor (LLS), the pump turns on.
When the water level reaches the High-Level Sensor (HLS), the pump turns off.
The pump remains on until the High-Level Sensor (HLS) is activated, ensuring the tank is filled to the desired level.

-----------------------------------------------------------------------------------------------------------
Ladder Logic Diagram
---------------------------------------------------------------------------------------------------------
|----[ I0.0 (LLS) ]----[ ]--------------------------------------( Q0.0 (Pump) )---|
|                            |                                                        |
|                            |                                                        |
|                            |----[ I0.1 (HLS) ]----[ ]---------------------------( Q0.0 (Pump) )---|

