---
aliases: 
tags:
  - architecture_synthesis
  - digital
  - design_synthesis
---
- The task is to assign the operation nodes of a [[Data Flow Graph|DFG]] to Control Steps (or Clock Cycles) under certain constraints and subject to the precedence constraint
- The constraints can be:
	- Hardware Resource
	- Operation Speed (Number of Clock Cycles)
- A high-level synthesiser can:
	- Optimize the **hardware** resource under the **speed** constraint
	- Optimize the **speed** resource under the **hardware** constraint

# Operation Scheduling Algorithms

（全是例子学个鸡毛）

![[Pasted image 20241029052640.png#pic_center|A DFG Example]]
## As Soon As Possible (ASAP)

所有资源都尽可能早地进入流水线。
![[Pasted image 20241029052658.png]]
## As Late As Possible (ALAP)

所有资源都尽可能晚地进入流水线。从最后一级倒退回去的遍历策略和ASAP一样。
![[Pasted image 20241029052719.png]]
## List Scheduling

- 根据一个Data Path上的节点数量来判断优先级，节点数量越多的一支优先级越高，越先进入流水线。
- 如果优先级一样，可以考虑其他的因素。
- 如果有空闲的资源会尽早利用上。
![[Pasted image 20241029052739.png]]
## Force Directed Scheduling
（喵）
## Integer Linear Programming Scheduling
（喵）