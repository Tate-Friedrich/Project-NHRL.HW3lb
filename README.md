# 3 lb NHRL Combat Robot – True Walker Horizontal Spinner

This repository documents the design and development of a 3 lb-class combat robot built for the **National Havoc Robot League (NHRL)**. The robot features a long horizontal spinning weapon and a fully compliant **true walker locomotion system**, allowing it to compete at a total weight of **6 lbs** under NHRL's walker rules.

Multiple alternate weapon and armor layouts are being considered as part of the design. NHRL rules allow up to 50% of a robot to be changed between fights, enabling modular optimization based on opponent matchups.

---

## Overview

- **Class:** 3 lb (True Walker – qualifies for 2x weight allowance)
- **Total Weight Limit:** 6 lbs
- **Mobility Type:** True Walker
- **Weapon Type:** Horizontal Spinner (primary configuration)

---

## Key Components

### Main Weapon Configuration
- **Motor:** [BadAss 3520-650Kv Brushless Motor](https://innov8tivedesigns.com/badass-3520-650kv-brushless-motor.html?srsltid=AfmBOopDLzuiBOnUxD94GPhQGZdmndHpF6OSiwQVLXf6bqlAEaklkeRaOdk&gQT=2)
- **Drive Method:** Belt-driven horizontal bar spinner
- Comparable weapon motors have been used successfully in 12 lb-class robots.

### Locomotion System
- **Servos (x4):** [Combat Robot Servo - 32kg-cm True 200 Degree with Stall Protection](https://justcuzrobotics.com/products/servo-32kg?_pos=10&_fid=a157f4870&_ss=c)
  - Wide-angle movement (200°) and high torque output.
  - Controlled by an **ESP32** microcontroller.
  - Powered directly by 4S LiPo batteries.
- Meets the **true walker** criteria with no rolling elements, qualifying for the full weight bonus.
  - Ideally 2 DoF legs allow for belly dragging reducing the weight needed for movement.

### Power System
- **Batteries (x2):** [GNB 850mAh 4S 15.2V LiHV LiPo](https://shop.robotsmashingleague.com/products/gnb-850mah-4s-15-2v-lipo-battery)
  - Powering both drive servos and the main weapon motor.
  - Batteries are connected in parallel for increased runtime at full voltage.

### Frame and Armor
- **Armor:** Predominantly **3D printed TPU** for flexible impact resistance. Titanium and aluminum plates will be integrated in critical areas as needed.
- **Top/Bottom Plates:** Cut from **aluminum** via CNC or waterjet processes to provide rigidity and mounting strength.
- Designed for quick disassembly and repair in tournament conditions.

---

## Alternate Weapon Configurations

Multiple interchangeable weapon designs are being toyed with to take advantage of NHRL’s allowance for 50% robot modularity:

- **Overhead Hammersaw**  
  A vertical disc or bar mounted on a swinging arm. Ideal for breaking into top armor or exposed electronics from above. Could be interesting given the weight bonus would allow for a faster weapon.

- **Double-Stacked Counter-Rotating Horizontal Spinner**  
  Two weapons rotating in opposite directions to reduce gyroscopic effects and potentially pinch enemies between the two spinning masses. Adds impact symmetry and reduces gyroscopic effects.

- **Dual Beater Bar System**  
  Taking a page from Verticalizer and putting two beater bars on a long Thagomizer style weapon arm. Ideally using the non-impacting weapon to kick the impacting bar hard into unsuspecting enemies.

---

## Goals

- Full compliance with NHRL’s true walker classification standards
- High-energy weapon delivery within the extended walker weight allowance
- Effective modularity for weapon and armor swaps between matches
- Rapid repairability and minimal downtime during events
- Controlled, programmable walking gait using servo-driven actuation

Ideally make a fun viable true walker.

---

## Development Progress

| Phase                         | Status         | Notes                                                                |
|-------------------------------|----------------|----------------------------------------------------------------------|
| Component Selection           | ✅ Complete    | Weapon motor, servos, power, and control electronics selected        |
| Inital CAD Design & Layout    | ⚙️ In Progress | Core chassis and weapon assemblies fully modeled                     |
| Final CAD Design & Layout     | ⚙️ In Progress | Core chassis and weapon assemblies fully modeled                     |
| Walker Gait Logic             | ⬜ Not Started || Initial servo sequencing and gait mapping underway                  |
| ESP32 Firmware                | ⬜ Not Started | PWM timing and movement logic under testing                          |
| Weapon Integration            | ⬜ Not Started | Awaiting fabrication of motor mounts and pulley hardware             |
| Electrical Wiring & Layout    | ⬜ Not Started | Final routing and component layout in progress                       |
| Armor Fabrication             | ⬜ Not Started | TPU prints queued, metal plate CAM files complete                    |
| Full Assembly                 | ⬜ Not Started | Dry fit and clearance check upcoming                                 |
| Functional Testing            | ⬜ Not Started | Spin-up, gait trials, and hit testing pending                        |
| Competition Prep              | ⬜ Not Started | Spares, weight check, and match travel kit TBD                       |

---

## Development Roadmap

### Component Selection and Initial Design  
- Major parts chosen including weapon motor, servo drive system, power configuration, and control electronics  
- CAD design and layout completed for core chassis and weapon assembly

### Mobility System Development  
- Walker gait strategy mapped for 2 DOF system  
- Control firmware being written and tested on ESP32 microcontroller  
- Load testing of servo behavior under walking sequences

### Weapon System Integration  
- Pulley geometry and belt tension design under review  
- Weapon mounting system designed to allow fast configuration changes  
- ESC and kill switch routing incorporated into internal layout

### Armor and Frame Fabrication  
- TPU impact armor sections in printing phase  
- Top and bottom aluminum plates to be waterjet cut and fitted  
- Assembly testing for screw clearance and internal spacing underway

### Electrical Integration and Testing  
- Wiring schematic finalized for dual battery setup and servo/ESC isolation  
- Bench tests scheduled for full system power draw and voltage stability  
- Kill switch, signal routing, and failsafe behavior verification

### Testing and Tuning  
- Controlled environment testing of walker locomotion and turn behavior  
- Weapon spin-up and balance testing under simulated match loads  
- Modular weapon swap time trials and armor fitting refinements

### Competition Readiness  
- Final weight verification and system checklist  
- Spare parts pack built including extra servos, belts, and armor panels  
- Travel configuration prepared for NHRL event debut with primary and alternate weapon options

---

## Repository Structure

