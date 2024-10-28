---
aliases:
  - 曼彻斯特进位链加法器
tags:
  - adder
  - digital
---
- [[Transmission-Gate-Based Adder]]中的Carry Gate可以通过[[Full Adder#中间信号|全加器的中间信号]]进一步简化。
- 表达式为：$C_o=G_i+P_iC_i$

# Static Logic

![[Static Manchester Carry Gates.png#pic_center|静态逻辑实现Manchester Carry Gates]]

- 进位传播路径不充电，如果进位传播信号$P=(A_i\oplus B_i)=1$，则$C_i$被传送至输出$C_o$
- 如果传播条件不满足，则输出由信号$D_i$下拉或$\overline{G_i}$上拉。

# Dynamic Logic

![[Dynamic Manchester Carry Gates.png#pic_center|动态逻辑实现Manchester Carry Gates]]

使用动态实现可以让电路更加简洁。由于动态电路中的晶体管是单方向工作的，所以可以只用NMOS传输管来代替传输门。预充电输出使电路不再需要进位取消信号（对于进位链，传播的是进位信号的反信号时的情景）。

# Dynamic Implementation of P and G

![[Dynamic Implementation of P and G.png#pic_center|动态逻辑中间信号产生电路]]
- Precharge when $\mathrm{Clk} = 0$
- [[Bleeder]] to compensate for the [[Charge Leakage]] due to the pull-down leakage paths

# 4-Bit Manchester carry Chain

- Uses pass transistors for carry chain
- All pass transistors are precharged to $V_{DD}(\phi=0)$
![[Pasted image 20241029035326.png#pic_center|4-Bit Manchester carry Chain]]