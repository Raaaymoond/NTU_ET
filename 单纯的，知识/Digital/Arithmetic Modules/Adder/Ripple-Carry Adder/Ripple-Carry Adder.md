---
aliases:
  - 行波进位加法器
  - 逐位进位加法器
tags:
  - adder
  - digital
---
![[Ripple-Carry Adder.png#pic_center|Ripple-Carry Adder]]


- An n-bit adder can be constructed by cascading n [[Full Adder]]s
- Ripple-Carry Adder is simple but suffer from long delay, specially when n is large.

# Delay

- For an n-bit Ripple-Carry Adder, the worst case delay occurs when a carry generated at LSB propagates all the way to MSB
$$t_{adder}=(n-1)\times t_{carry}+t_{sum}$$
- $t_{carry}$: propagation delay from $C_i$ to $C_o$
- $t_{sum}$: propagation delay from $C_i$ to $S$

- For 8-bit addition, one of the worst case delay occurs when $a=011111111b$ and $b=00000001b$
$$a+b=01111111b+00000001b=10000000b$$
