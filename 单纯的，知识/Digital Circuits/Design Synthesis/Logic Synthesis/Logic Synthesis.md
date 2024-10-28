---
aliases: 
tags:
  - design_synthesis
  - digital_circuits
  - TODO
---
- Logic Synthesis generates a gate-level implementation (structure view) of a logic function (logic-level view)
- The logic function can be specified in terms of state transition diagrams, schematics, Boolean equations, truth table or HDL descriptions
- Synthesis results depend on the implementation architecture: multilevel logic, PLA, FPGA/CPLD

# Logic Synthesis Tasks

- The objective of logic synthesis is to optimize the area, speed, power, or their combination
- The task has two main stages:
	- Logic minimization: a technology independent phase, where the logic is optimized using a number of Boolean algebraic manipulation techniques.
	- Technology mapping: a phase considers the implementation architecture, such as standard cells, PLA, FPGA/CPLD, etc.

# Combinational Logic Synthesis

将原始的表达式转换为使用更加简单逻辑门的形式（例如异或转换为OR-AND-NOT）
# Sequential Logic Synthesis

- State Minimization: Two states are equivalent if the output sequences for any input are the same
- State Encoding: Different code assignment for the states can result in different logic implementation
- State Machine Decomposition: Dividing a large state Machine into 2 or more small ones. Logic will be simpler and easier to be minimized. Speed can be increased too.
- **Retiming**: The clock speed depends on the delay between any two stages of a sequential circuit. By rearranging the sequential logic elements (flip flops), the delay can be reduced.
