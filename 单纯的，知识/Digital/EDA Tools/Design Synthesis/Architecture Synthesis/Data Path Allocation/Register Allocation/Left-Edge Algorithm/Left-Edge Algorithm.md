---
aliases: 
tags:
  - digital
  - design_synthesis
  - architecture_synthesis
  - data_path_allocation
  - register_allocation
---

- 将所有值的生命周期按照左端点排序列在表中。
- 遍历整个列表，不断选择没有重复的段，并合并

![[Pasted image 20241029052908.png#pic_center|Lifetime Table]]
- 上图中，所有值都按照左序排列
- 其中e1，e3，e4没有重复，所以可以合并到一个寄存器R1中
- 其他的值也是这么操作。