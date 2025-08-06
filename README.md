# Food Storage Robot

---

## Table of Contents

- [Overview](#overview)
- [Robot Selection](#robot-selection)
- [Motors](#motors)
- [Working Area](#working-area)
  - [Working Envelope](#working-envelope)
  - [Operating Area](#operating-area)
  - [Dead Zone](#dead-zone)
- [Safety Considerations](#safety-considerations)
  - [Emergency Stop](#emergency-stop)
  - [Maintenance](#maintenance)
- [Conclusion](#conclusion)

---

## Overview

This is Task Two in the Mechanical Engineering track, submitted to Smart Methods Company for 2025 Summer Internship. The task focuses on proposing a theoretical algorithm for an autonomous robotic system to automate food storage in a warehouse. The algorithm includes robot selection, motor requirements, working area definitions, and safety considerations for full automation without human intervention.

---

## Robot Selection 

From my perspective, I suggest delta robot due to the following characteristics: 

| No. | Characteristic      | Details                                                                 |
|-----|---------------------|-------------------------------------------------------------------------|
| 1   | 3-DOF               | Can move in multiple directions (X, Y, Z) with fast and precise linear motion. |
| 2   | High Speed          | Capable of rapid pick-and-place operations.                            |
| 3   | Precision           | Symmetrical structure allows for accurate positioning                  |
| 4   | Low- Inertia        | With motors located on the base, the arms remain lightweight, allowing for fast, energy-efficient movement. |
| 5   | Clean and Compact Design | Easy to sanitize, making it suitable for food-grade environments.        |

**Table 1: Reasons**

<p align="center">
  <img src="Delta Robot.jpg" alt="Delta Robot" />
</p>
<p align="center"><strong>Figure 1: Delta Robot</strong></p>

---

## Motors

The Delta robot requires three servo motors for its operation — one for each arm. The recommended type is brushless DC servo motors (BLDC). These motors are selected due to the following advantages:

- High efficiency and smooth operation  
- High torque-to-weight ratio, enabling fast and precise motion  
- Long lifespan and low maintenance, which is important for continuous industrial use  
- Excellent speed control and positional accuracy due to built-in high-resolution encoders  

<p align="center">
  <img src="BLDC Motor.jpg" alt="BLDC Motor" />
</p>
<p align="center"><strong>Figure 2: BLDC Motor</strong></p>

---

## Working Area 

For this system, I suggest the working area as a rectangular zone that includes:

- Storage shelves containing food items  
- A Delta robot mounted above a central conveyor belt  
- The conveyor belt is used for transferring food packages between stations: packing, sorting, storage.

The working area is divided into three important technical regions:

### Working Envelope 

This refers to the maximum volume within which the Delta robot can move its end-effector. Since Delta robots have a dome-shaped working envelope, the design ensures all items on the conveyor within that dome can be reached for sorting or picking. The envelope radius and height depend on the robot's arm lengths.

### Operating Area 

This is the entire area where robot-related activities happen. It includes:

- The conveyor belt area where food arrives and departs.  
- The pick-and-place zones under the Delta robot.  
- The space near the shelves where food packages are temporarily stored.  

### Dead Zone 

These are areas outside the robot’s reach, typically at the corners of the shelves or conveyor, where the Delta robot cannot operate. These zones are considered during design to ensure all items fall within the robot's reachable range. Additionally, dead zones include safety buffer areas where no robot movement occurs to avoid collision or overextension.

---

## Safety Considerations

The two primary safety parameters to consider in designing the autonomous food storage robot are: Emergency Stop and Maintenance. 

### Emergency Stop

A clearly accessible emergency stop button must be installed to immediately shut down the robot in case of malfunction, unexpected human presence, or other hazards. It prevents potential accidents and protects both equipment and personnel.

### Maintenance 

The system should include lockout/tagout procedures to ensure the robot cannot be powered on during maintenance. The design must also allow safe access to components for routine inspection, cleaning, and repair without risk of injury.

---

## Conclusion 

In conclusion, this task outlines a theoretical design for an autonomous food storage robot using a Delta Robot. For future work, I will focus on building and simulating the system in SolidWorks to move toward real-world implementation.
