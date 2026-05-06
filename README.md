# Digital Kinetic Clock

A mechanical digital clock built using servo motors, 3D-printed components, rack-and-pinion mechanisms, and an Arduino Mega microcontroller. The project combines mechanical motion with electronics to create a physical 7-segment digital clock where each segment moves dynamically using servo actuation.

---

## Project Overview

The Digital Kinetic Clock is an engineering project focused on combining:
- Mechanical design
- Embedded systems
- Servo motor control
- Real-time clock synchronization
- 3D printing and fabrication

Unlike conventional LED-based digital clocks, this clock physically moves mechanical segments to display time.

The project uses:
- Servo motors for segment movement
- Rack-and-pinion mechanisms
- DS3231 RTC module for accurate timekeeping
- Arduino Mega for control logic
- 3D-printed modular components

The system continuously reads the current time from the RTC module and dynamically actuates servos to display the correct digits.

---

## Features

- Mechanical 7-segment display
- Real-time clock synchronization
- Smooth servo-based motion
- Modular snap-fit assembly
- Rack-and-pinion mechanism
- Arduino-based control system
- Servo calibration system
- Power-efficient servo detachment logic

---

## Technologies & Components Used

### Hardware
- Arduino Mega
- DS3231 RTC Module
- Servo Motors
- Rack and Pinion Mechanism
- 3D Printed Components
- CO2 Laser Cut Parts

### Software
- Arduino IDE
- Embedded C / Arduino Programming

### Fabrication
- 3D Printing
- Laser Cutting
- CAD Modeling

---

## Mechanical Design

The clock was designed using modular snap-fit components for:
- Easier assembly
- Quick prototyping
- Better alignment
- Simple maintenance

Each digit consists of:
- 7 moving segments
- Servo-actuated linear motion
- Rack-and-pinion transmission system

The main body includes:
- Four digit panels
- Colon separator panel
- Sliding back plate
- Servo brackets

---

## Working Principle

1. The DS3231 RTC module provides real-time data.
2. Arduino reads the current time.
3. Each digit is mapped to a 7-segment representation.
4. Servo motors rotate according to required segment states.
5. Rack-and-pinion mechanisms convert rotational motion into linear motion.
6. Segments move physically to display numbers.

---

## Assembly Process

### Step 1: 3D Modeling
- CAD models created for:
  - Servo brackets
  - Segments
  - Gears
  - Face panel
  - Back panel

### Step 2: Servo Mounting
- Servos mounted using brackets and screws.

### Step 3: Panel Assembly
- Segment panels inserted into main body.

### Step 4: Wiring
- Servos connected to Arduino Mega.
- RTC module connected using I2C communication.

### Step 5: Calibration
- Servo intervals calibrated for accurate segment positioning.

### Step 6: Programming
- Arduino code uploaded to control servo motion and time display.

---

## Wiring Connections

### RTC Module Connections

| RTC Pin | Arduino Mega Pin |
|---------|------------------|
| SDA     | Pin 20 (SDA)     |
| SCL     | Pin 21 (SCL)     |

---

## Servo Pin Mapping

- First Digit → Starts at Pin 2
- Second Digit → Starts at Pin 9
- Third Digit → Starts at Pin 22
- Fourth Digit → Starts at Pin 29

---

## Repository Structure

```bash
├── Arduino_Code/
├── CAD_Designs/
├── Images/
├── README.md
```

---

## Servo Calibration

Since low-cost servo motors have slight positional inaccuracies, calibration intervals were implemented to:
- Align segments properly
- Improve display symmetry
- Ensure smooth motion

The calibration values are stored in arrays inside the Arduino code.

---

## Challenges Faced

### 1. Poor 3D Print Quality
- Difficult support removal
- Dimensional inaccuracies

### 2. Improper Part Fitting
- Components required manual adjustment

### 3. Rack-and-Pinion Meshing Issues
- Laser cutter produced bevel-like edges

### 4. RTC Battery Discharge
- Required recalibration after battery drain

### 5. Servo Shaft Damage
- Accidental glue spill caused movement issues

---

## Solutions Implemented

- Improved error-tolerant design
- Better fabrication calibration
- CO2 laser cutting for improved precision
- Reduced glue dependency
- Added servo calibration logic
- Suggested physical buttons for future RTC setup

---

## Future Improvements

- Wireless time synchronization
- Mobile app integration
- Better quality servo motors
- PCB-based compact electronics
- CNC-machined precision gears
- Automatic RTC synchronization
- Touch/button-based time adjustment

---

## Applications

- Mechanical display systems
- Embedded systems learning
- Mechatronics projects
- Interactive installations
- Educational demonstrations
- Smart desk clocks

---

## Key Learning Outcomes

- Real-world manufacturing challenges
- Servo motor control
- Embedded programming
- Mechanical-electrical integration
- CAD design and prototyping
- Calibration and motion control

---

## Team Members

- Sneha
- Rahul
- Dhaval
- Yash

---

## Author

**Dhaval Nikam**  
B.Tech Project  
Indian Institute of Technology Goa

---

## References

- DS3231 RTC Documentation
- Arduino Servo Library
- Embedded Systems Design Concepts
- Mechanical Rack-and-Pinion Mechanisms

---

## License

This project is developed for educational and academic purposes.
