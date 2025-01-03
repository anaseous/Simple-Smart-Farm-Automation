# The project will:
  Monitor soil moisture levels using a sensor.
  Automate irrigation by controlling a water outlet (e.g., a solenoid valve).
  Display a dashboard in Node-RED for monitoring and manual override.

## Components Needed:
# 1. Hardware:
  - Soil Moisture Sensor (e.g., Capacitive Soil Moisture Sensor v1.2).
  - Solenoid Valve (e.g., Rainbird or similar 12V DC water valves).
  - Relay Module (to control the solenoid valve).
  - Raspberry Pi (for running Node-RED).
  - Power Supply (matching the solenoid valve voltage).

# 2. Software:
    Node-RED installed on Raspberry Pi.
    Additional Node-RED nodes for dashboard and GPIO control.

# 3. Circuit Connection
    1. Soil Moisture Sensor:
      Connect the sensor to the analog input of an ADC module (e.g., MCP3008) as Raspberry Pi does not have analog inputs.
      Power the sensor with 3.3V or 5V.
# 4. Relay Module:
      Connect the relay module to the GPIO pins of the Raspberry Pi.
      Wire the solenoid valve to the relay module.

# 5. Node-RED Flow
    Here’s the logic for the irrigation system:
    1. Monitor soil moisture levels.
    2. Compare moisture levels against a threshold (e.g., 30%).
    3. Turn the solenoid valve ON if below the threshold, OFF if above.
    4. Display a dashboard with:
      Real-time soil moisture readings.
      Status of the valve (ON/OFF).
      Manual override button.
6. Recommended Solenoid Valve
    Rainbird 100-DVF: Durable and commonly used in irrigation.
    Hunter PGV: Efficient and reliable for small-scale smart farms.
    Amazon Basics Solenoid Valve: Budget-friendly options available online.
