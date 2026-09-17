# Week 8

**Goal this week:** Test and finalize the perfboard-based electrical system, integrate all the major components into the 3D-printed rover base, and begin room-based testing of the ultrasonic sensors to obtain accurate measurements for future mapping and autonomous navigation.

## What we did

- This week, we tested the completed perfboard circuit to verify that all the connections were working correctly and that the components were receiving the required power.
- The perfboard assembly consisted of the Arduino Uno, buck converter, Bluetooth module, ultrasonic sensors, motor driver and motor connections. All the components were arranged and soldered properly to make the circuit compact and reliable.
- After testing the individual connections, we fixed the perfboard and the other components into the 3D-printed rover base. The components were positioned carefully to maintain a neat arrangement and to prevent the wires from interfering with the mechanical parts.
- We connected the complete system to the 14.8 V battery through the appropriate power arrangement and tested whether each component was functioning properly.
- The Arduino Uno was tested to ensure that it was communicating correctly with the Bluetooth module and controlling the motor driver.
- The motor driver and motors were tested to verify that the rover could move correctly after transferring the connections from the breadboard to the permanent perfboard.
- The ultrasonic sensors were also connected and tested with the Arduino Uno. We checked whether they were able to detect obstacles and provide distance measurements correctly.
- After confirming that the major components were working, we started testing the rover inside a room environment. This was done to understand the actual distance measurements obtained from the ultrasonic sensors under practical conditions.
- We tested the sensors at different positions and distances from walls and other obstacles to identify suitable sensor placement and obtain more accurate measurements.
- These measurements will be useful during the mapping stage, as the rover needs to cover the required distance accurately and the ultrasonic sensors need to detect obstacles at the correct points during movement.
- The testing also helped us identify and correct minor wiring and positioning issues before proceeding to the mapping and autonomous navigation stage.

## Problems and blockers

- Testing the complete perfboard required checking multiple connections because all the components were permanently soldered together.
- Proper placement of the components inside the 3D-printed base was challenging because limited space was available for the circuit, battery connections and wiring.
- The ultrasonic sensor readings could vary depending on the position and distance of the sensor from walls and obstacles.
- Accurate distance measurement was important because incorrect sensor readings could affect obstacle detection and the accuracy of the mapping process.
- The rover had to be tested multiple times in the room to determine suitable sensor positions and understand how accurately the sensors detected obstacles.

## Decisions

- We decided to use the perfboard as the main permanent circuit instead of the temporary breadboard setup.
- We decided to mount the Arduino Uno, buck converter, Bluetooth module, motor driver and other components securely inside the 3D-printed rover base.
- We decided to keep the wiring as neat and compact as possible to make the rover easier to maintain and reduce the possibility of loose connections.
- We decided to test the ultrasonic sensors in an actual room environment before starting the mapping process.
- We decided to collect and verify accurate distance measurements so that the rover can detect obstacles at the expected positions during mapping and autonomous navigation.
- We decided to complete the electrical and mechanical testing before moving to the full mapping and autonomous operation stage.

## Next week

- Continue testing and calibrating the ultrasonic sensors for more accurate distance measurements.
- Start implementing and testing the room mapping system.
- Test the rover's movement over predefined distances.
- Integrate ultrasonic obstacle detection with the rover's movement.
- Begin testing autonomous navigation based on the mapped environment.
- Identify and correct any issues found during mapping and autonomous movement.
- Continue improving the overall reliability and compactness of the rover system.

## Links

- Code:
- Photos / CAD:
