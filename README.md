# 3 lb NHRL Combat Robot – True Walker Horizontal Spinner

This repository documents the design and development of a 3 lb-class combat robot built for the **National Havoc Robot League (NHRL)**. The robot features a long horizontal weapon and a fully compliant **true walker locomotion system**, allowing it to compete at a total weight of **24 lbs** under NHRL walker rules. I do plan on including alternate weapon and armor layouts as 

---

## Overview

- **Class:** 3 lb (True Walker – qualifies for 2x weight allowance)
- **Total Weight:** 6 lbs
- **Mobility Type:** True Walker
- **Weapon Type:** Horizontal Spinner

---

## Key Components

### Weapon System
- **Motor:** [BadAss 3520-650Kv Brushless Motor](https://www.maxamps.com/badass-3520-650kv-brushless-aeromodel-motor)
- **Drive Method:** Belt-driven horizontal bar spinner
- The motor should provide more than enough power for the weightclass. Missouri S&T runs a vertical robot at 12lbs with a comparable motor.
- Ideally multiple weapon loadouts could be used as NHRL allows for up to 50% of the robot to be changed in different layouts.

### Locomotion System
- **Servos (x4):** [Combat Robot Servo - 32kg-cm True 200 Degree with Stall Protection](https://justcuzrobotics.com/products/combat-robot-servo-32kg-true-200-degree-with-stall-protection)
  - Each servo offers high torque output and wide-angle control.
  - Originally intended for flippers, they should provide more than enough power for walking motion.
  - Controlled by an **ESP32** microcontroller.
  - Directly powered by a 4S LiPo battery.
- This configuration meets the **true walker** definition by moving without rolling elements, qualifying for the 2x weight bonus.

### Power System
- **Batteries (x2):** GNB 850mAh 4S 15.2V LiHV LiPo
  - These batteries supply power for both the drive servos and the weapon motor.

### Frame and Armor
- **Armor:** Primarily **3D printed TPU** for impact absorption and flexibility. Ti and Aluminum plates to be added as needed.
- **Top and Bottom Plates:** CNC-machined or waterjet-cut **aluminum** for structural strength and durability.
- The frame is designed to minimize weight while offering modular replaceability for rapid pit repairs.

---

## Goals

- Fully compliant with NHRL’s true walker classification.
- Maximize effective weapon energy within the walker weight bonus.
- Prioritize repairability and modular design for quick between-match fixes.
- Demonstrate the viability of high-torque servo-driven true walking mechanisms in competition.

---

## Roadmap

- [x] Component selection
- [X] CAD design and prototyping
- [ ] Walker gait testing and tuning
- [ ] Weapon spin-up and control integration
- [ ] Armor print and assembly
- [ ] Field testing
- [ ] NHRL competition debut


