---
aliases:
  - 互补CMOS全加器
tags:
  - adder
  - digital
  - arthmetic_modules
---
由[[Full Adder]]改进而来。
# 表达式

$$C_o=AB+BC_i+AC_i$$
$$S=A\oplus B \oplus C_i=ABC_i+\overline{C_o}(A+B+C_i)$$
# Drawbacks

- The Complementary Static CMOS full adder cell has 28 transistors.
- It is large and slow.
- PMOS stacks are in carry and sum part.
- Intrinsic capacitance of co is large: 6 [[Gate Capacitance]] + 2 [[Diffusion Capacitance]] + Interconnect Capacitance.
- Carry propagates through 2 inverting stages.
- Sum output requires extra logic (although not critical).

# Improvement

Remove an inverter of the carry chain
![[Pasted image 20241021201112.png#pic_center|改进的进位链]]