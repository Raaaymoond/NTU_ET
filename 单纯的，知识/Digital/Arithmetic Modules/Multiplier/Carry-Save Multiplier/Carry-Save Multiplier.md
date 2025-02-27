---
aliases:
  - 进位保留乘法器
tags:
  - multiplier
  - digital
  - arthmetic_modules
---
![[Carry-Save Multiplier_1.png|Carry-Save Multiplier]]

- Carry is fed to the [[Full Adder]] of the next level
  进位被传递到下一层的全加器

在[[Array Multiplier|阵列乘法器]]中，通过在最后一级添加向量合并（vector-merging）加法器，进位路径可以通过对角线传输。在进位保留乘法器中，进位并不立即相加，而是保留给下一级加法器。在最后一级，进位与和在一个加法器（CPA，超前进位、进位旁路）中合并。

# Delay

进位保留乘法器在最坏情况下关键路径最短，并且唯一确定，传播延时为：
$$t_{\text{p}}=t_{\text{and}}+(N-1)\cdot t_{\text{carry}}+t_{\text{merge}}$$
上式中假设$t_{\text{add}}=t_{\text{carry}}$

# Carry-Save Multiplier Floorplan

可以画成长方形，注意图中的规律。
![[Carry-Save Multiplier_2.png|Rectangle floorplan of carry-save multiplier]]