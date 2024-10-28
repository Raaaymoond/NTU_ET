---
aliases: 
tags:
  - lecture_slides
  - Ivan
---
# Generic Digital System

A Generic Digital System consists of:
- [[Datapath]]
- [[Control Unit]]
- [[Memory]]
- [[Input Output]] Modules
![[Pasted image 20241029022848.png#pic_center|Generic Digital System]]

# Arithmetic Modules

- Datapath in digital systems consists of mainly arithmetic modules
- Common arithmetic modules include [[Adder]]s (Subtractor), [[Multiplier]]s, [[Shifter]]s

# Power Considerations in Datapath

- To compensate the reduction of speed, design techniques can be used
- Parallel functional blocks operate at lower frequency and lower $V_{DD}$ can be used to process data in parallel to compensate loss of performance
- Pipeline structure of functional blocks can also be used to save power as lower $V_{DD}$ is needed to charge smaller capacitance for the same speed

## Clock Gating

- [[Clock Gating]]

## Power Gating

- [[Power Gating]]

## Other Low Power Techniques

- [[Multiple Supply Voltages]]
- [[Dynamic Voltage and Frequency Scaling]]
- [[Power-down Mode]]

# Design Complexity #TODO 

## Intel Microprocessors

## Moore’s Law

- Gordon Moore:
	- Fairchild Corporation
	- Cofounder of Intel
- Prediction in 1965: **“The number of transistors incorporated in a chip will approximately double every 24 months.”**

# Design Abstraction Levels #TODO 

![[Pasted image 20241029043505.png#pic_center|Design Abstraction Levels]]

## Gajski-Kuhn Y Diagram

### Objects In Each Domain

# Design Hierarchy

# Design Entry

- Text based Hardware Description Languages
	- VHDL
	- Verilog
- Schematics
- State Diagram
- Flow Chart

# Synthesis, Partitioning & Simulation

- Logic Synthesis
	- Use synthesis tools to translate HDL to a netlist of logic gates and their connections
- System Partitioning
	- Divide a large system into smaller blocks
	- Several ICs if necessary
- Prelayout Simulation
	- Verify the functionality of the system

# Floorplanning, Placement & Routing

- Floorplanning
	- Arrange the blocks of the design to optimize the size and the interconnections
- Placement
	- Decide the locations of modules and logic cells
- Routing
	- Make connection between cells and modules

# Extraction & Postlayout Simulation

- Extraction
	- Convert the layout back to circuits
	- Determine the resistance and capacitance of the interconnect
- Postlayout Simulation
	- Verify the functionality again, with the added loads of the interconnect
	- Verify the timing

# EDA Tools

4 Main Categories:
- [[Ivan Lecture Slides#Design Entry Tool|Design Entry]]
- [[Analysis]] and [[Verification]]
- [[Design Synthesis|Synthesis]] and Implementation
- Testing

## Design Entry Tool

- Schematic Editor
	- **Cell Library**: Contains components to be used
	- **Editing Functions**: Place, Move, Delete, Connect, Rotate/Flip, Copy/Paste
	- **Hierarchical Design**: Modules contain lower-level schematics
	- **Netlist Description Language**: Electronic Design Interchange Format (EDIF)

# Hierarchical Schematic 

![[Pasted image 20241029044315.png]]
- (a) [[Half Adder|HADD]] Schematic
- (b) Schematic Symbol
- (c) Higher-level Schematic that makes use of [[Half Adder|HADD]]
- (d) Hierarchy of [[Half Adder|HADD]]

# Implementation Approaches

![[Pasted image 20241029050258.png#pic_center|Implementation Approaches]]

# Design Synthesis

- [[Design Synthesis]]

