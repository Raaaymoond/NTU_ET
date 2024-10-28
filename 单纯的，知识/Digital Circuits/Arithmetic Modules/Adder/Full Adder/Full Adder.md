---
aliases:
  - 全加器
tags:
  - adder
  - digital_circuits
---

- A Full Adder (FA) has 2 adder inputs ($A$, $A$), 1 carry input ($C_i$), a sum output ($S$) and a carry output ($C_o$)
- Boolean equations are:$$S=A\oplus B \oplus C_i$$ $$C_o=AB+BC_i+AC_i$$

# Truth Table

| $a$ | $b$  | $c_i$ | $s$  | $c_o$ |
| :-: | :-: | :---: | :-: | :---: |
|  0  |  0  |   0   |  0  |   0   |
|  0  |  0  |   1   |  1  |   0   |
|  0  |  1  |   0   |  1  |   0   |
|  0  |  1  |   1   |  0  |   1   |
|  1  |  0  |   0   |  1  |   0   |
|  1  |  0  |   1   |  0  |   1   |
|  1  |  1  |   0   |  0  |   1   |
|  1  |  1  |   1   |  1  |   1   |

# 中间信号

可以把$S$和$C_o$定义由某些中间信号产生的信号。这些中间信号包括：
- $G=AB$ 进位产生（carry dgenerate）信号
- $D=\overline{A}\ \overline{B}$ 进位取消（carry ddelete）信号
- $P=A\oplus B$ 进位传播（carry dpropagate）信号

# Inverting Property of Adder Cell

Adder cell has an Inverting property
$$\overline{S}(A,B,C_i)=s(\overline{A},\overline{B},\overline{C_i})$$
$$\overline{C_o}(A,B,C_i)=C_o(\overline{A},\overline{A},\overline{C_i})$$
根据这一性质可以设计[[Complementary Static CMOS Full Adder Cell]]