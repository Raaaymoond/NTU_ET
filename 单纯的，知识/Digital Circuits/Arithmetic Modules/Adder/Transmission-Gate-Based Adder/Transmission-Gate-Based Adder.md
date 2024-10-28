---
aliases:
  - 传输门型加法器
tags:
  - adder
  - digital_circuits
---

全加器可以用多路开关和XOR门设计
![[Transmission-Gate-Based Adder.png#pic_center|使用传输门和XOR门设计全加器]]

# 表达式

[[Full Adder#中间信号|全加器的中间信号]]：
$$P=A_i \oplus B_i$$

输出：
$$S=P\oplus C_i=\overline{\overline{P}\ \overline{C_i}+PC_i}$$
$$C_o=A_iB_i+PC_i=\overline{\overline{P}\ \overline{A_i}+P\overline{C_i}}$$

# 特点

- 和与进位输出有近似的延时