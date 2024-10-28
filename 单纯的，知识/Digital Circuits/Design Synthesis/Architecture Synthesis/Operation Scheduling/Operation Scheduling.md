---
aliases: 
tags:
  - architecture_synthesis
  - digital_circuits
  - design_synthesis
---
- The task is to assign the operation nodes of a [[Data Flow Graph|DFG]] to Control Steps (or Clock Cycles) under certain constraints and subject to the precedence constraint
- The constraints can be:
	- Hardware Resource
	- Operation Speed (Number of Clock Cycles)
- A high-level synthesiser can:
	- Optimize the hardware resource under the speed constraint
	- Optimize the hardware resource under the speed constraint

# Algorithms

（全是例子学个鸡毛）

## As Soon As Possible (ASAP)

所有资源都尽可能早地进入流水线。

## As Late As Possible (ALAP)

所有资源都尽可能晚地进入流水线。从最后一级倒退回去的遍历策略和ASAP一样。

## List Scheduling

- 根据一个Data Path上的节点数量来判断优先级，节点数量越多的一支优先级越高，越先进入流水线。
- 如果优先级一样，可以考虑其他的因素。
- 如果有空闲的资源会尽早利用上。

## Force Directed Scheduling

（喵）

## Integer Linear Programming Scheduling

（喵）