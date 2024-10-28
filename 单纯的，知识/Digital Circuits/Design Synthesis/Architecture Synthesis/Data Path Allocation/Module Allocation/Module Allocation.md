---
aliases: 
tags:
  - digital_circuits
  - design_synthesis
  - architecture_synthesis
  - data_path_allocation
---
- Operations are bound to physical functional module during the Module Allocation stage
- The number of modules have been determined in the scheduling state
- Different bindings will result in different interconnects (including MUX, bus, wires)
- [[Register Allocation]] and [[Module Allocation]] are interdependent
- They influence the [[Interconnect Allocation]] results