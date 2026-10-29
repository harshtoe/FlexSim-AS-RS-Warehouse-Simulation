# FlexSim AS/RS Warehouse Simulation

Discrete-event simulation of an automated storage and retrieval system (AS/RS) built in FlexSim. The project compares three slotting strategies to see how they affect crane and warehouse performance.

## Overview
- 8 storage racks served by ASRS cranes
- Conveyor-fed inbound flow and outbound flow to a sink
- Logic built with FlexSim Process Flow: base stock creation, inbound putaway, and order-driven outbound retrieval (ASRS tasks)

## Scenarios
1. **Random Placement**: pallets assigned to any available slot
2. **Static ABC Slotting**: SKUs assigned to zones by classification
3. **Dynamic Zone Balancing**: slot and crane selection balanced across zones

Only the `Find Slot` and crane-selection nodes change between scenarios. The physical crane execution nodes stay the same, so differences in results come from the slotting logic alone.

## Input Data
| File | Purpose |
|---|---|
| `SKU_Master` | SKU attributes |
| `Base_Stock` | Initial inventory |
| `Inbound_Schedule` | Inbound pallet arrivals |
| `Outbound_Orders` | Retrieval orders |

## Results
<img width="1295" height="790" alt="asrs 1" src="https://github.com/user-attachments/assets/d58370e3-5ddc-4940-a83d-332cf6101866" />


## Tools
FlexSim, Process Flow, Excel/CSV data inputs

## Author
Harsh, B.Tech Production Engineering
