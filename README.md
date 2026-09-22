# line-following-robot
ESP32-based line-following robot using IR sensors and a motor driver for autonomous path tracking.


| Component             |  Quantity |
| --------------------- | --------: |
| ESP32 Dev Kit         |         1 |
| IR Sensor Module      |         2 |
| DC Motors + Wheels    |         4 |
| Motor Driver (L298N)  |         1 |
| 18650 Li-ion Battery  |         3 |
| BMS Module            |         1 |
| Switches, Wires, Base | As needed |


## How It Works

- IR sensors detect the black line on a white surface.
- The ESP32 continuously reads the sensor values.
- The ESP32 processes the sensor inputs and controls the motors through the L298N motor driver.
- If both sensors detect white, the robot moves forward.
- If the left sensor detects black, the robot turns right.
- If the right sensor detects black, the robot turns left.
- If both sensors detect black, the robot stops.
