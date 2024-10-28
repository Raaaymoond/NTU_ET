---
aliases: 
tags:
  - lecture_slides
  - Ivan
  - digital
  - TODO
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

![[Pasted image 20241029061001.png|Gajski-Kuhn Y Diagram]]

 ### Objects In Each Domain

|                    |                     Behavioural                      |                 Structural                  |        Physical        |
| :----------------: | :--------------------------------------------------: | :-----------------------------------------: | :--------------------: |
|       System       |                  Performance Specs.                  |  CUPs<br>Memories<br>Controllers<br>Buses   |  Physical Partitions   |
|    Algorithmic     |                   Data Procedures                    |     Hardware Modules<br>Data Structures     |        Clusters        |
| Microarchitectural | Operations<br>Register Transfers<br>State Sequencing | ALUs<br>MUXs<br>Registers<br>Microsequencer |       Floorplans       |
|       Logic        |               Boolean Equations<br>FSM               |        Gates<br>Flip-Flops<br>Cells         | Cell /<br>Moudle Plans |
|      Circuit       |             Transfer Functions<br>Timing             |      Transistors<br>Wires<br>Contacts       |         Layout         |

# Design Hierarchy

![[Pasted image 20241029055425.png#pic_center|Design Hierarchy]]

## Design Flow

![[Pasted image 20241029055457.png|Design Flow]]

### Design Entry

- Text based Hardware Description Languages
	- VHDL
	- Verilog
- Schematics
- State Diagram
- Flow Chart

### Synthesis, Partitioning & Simulation

- Logic Synthesis
	- Use synthesis tools to translate HDL to a netlist of logic gates and their connections
- System Partitioning
	- Divide a large system into smaller blocks
	- Several ICs if necessary
- Prelayout Simulation
	- Verify the functionality of the system

### Floorplanning, Placement & Routing

- Floorplanning
	- Arrange the blocks of the design to optimize the size and the interconnections
- Placement
	- Decide the locations of modules and logic cells
- Routing
	- Make connection between cells and modules

### Extraction & Postlayout Simulation

- Extraction
	- Convert the layout back to circuits
	- Determine the resistance and capacitance of the interconnect
- Postlayout Simulation
	- Verify the functionality again, with the added loads of the interconnect
	- Verify the timing

# EDA Tools

4 Main Categories:
- [[Design Entry Tool|Design Entry]]
- [[Analysis]] and [[Verification]]
- [[Design Synthesis|Synthesis]] and [[Implementation]]
- Testing
