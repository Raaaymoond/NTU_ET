# Memories

![[Pasted image 20241105174221.png#pic_center|]]

- Data storage needs Random-access memory (RAM), and Read-only memory (ROM), high speed and high density
  数据存储需要随机存取存储器 (RAM) 和只读存储器 (ROM)，高速且高密度
- The 1st RAM was invented in the mid-1960s
  第一个RAM在1960年中叶被发明
- The 1st commercial 1024-bit (1-Kb) RAM was introduced in 1974.
  第一个商用的1kb RAM在19174年发明

## Random Access Memory (RAM)

- Random Access Memory (RAM) refers to the memory in a digital system that has both read and write capabilities.
  随机存取存储器 (RAM) 指的是数字系统中具有读写功能的存储器
- Static RAM (SRAM) is able to store information as long as power is applied, and they will not lose their data during a read cycle.
  静态随机存取存储器 (SRAM) 在通电时能够持续存储信息，并且在读取周期中不会丢失数据
- Dynamic RAM (DRAM) uses a capacitor to temporarily store data which must be refreshed periodically to prevent information loss.
  动态随机存取存储器 (DRAM) 使用电容器来临时存储数据，必须定期刷新以防止信息丢失

### Block Diagram of A Basic Memory Array

![[Pasted image 20241105175548.png#pic_center|]]
- Horizontal rows are called wordlines while the vertical lines are called bitlines
  水平的被称为字线，竖直的被称为位线
- The cell arrays contains $2^{M+N}$ storage locations (cells).
  单元阵列包含$2^{M+N}$ 个存储位置（单元）。

- **Row and column address decoders** are required to select desired row and column
  **行和列地址解码器**用来选择所需的行和列。
- **Wordlines (WL)** They are the horizontal rows with a number of $2^M$
  **字线 (WL)** 具有$2^M$个水平行。
- **Bitlines (BL)** They are the columns with a number of $2^N$. They contain the cell data
  **位线**有$2^N$列，它们含有单元的数据
- The selected **BL** by the address decoder can transfer the data to the output during read operation, or modify the data during a write operation
  由地址解码器选择的**位线**可以在读取操作时将数据传输到输出，或在写入操作时修改数据
- **Sense Amplifiers** They are connected to the BLs. They are required to detect the state of the memory cell and restore the signal to a full logic level
  **感应放大器**连接到位线。它们用于检测存储单元的状态并将信号完全恢复到逻辑电平

### SRAM Cells

#### Two Inverter Latch

![[Pasted image 20241105205301.png]]
- Inverters configured as shown in the above figure form the basic static storage building block
  如上图所示配置的反相器构成了基本的静态存储组件
- These cross-coupled inverters are often referred to as a latch
  这些交叉耦合的反相器通常被称为锁存器

![[Pasted image 20241105205544.png#pic_center]]
- The latch usually has only two stable states termed bistable
  锁存器通常只有两个稳定状态，称为双稳态
- However, it is possible for it to enter an unstable equilibrium point where $v_I=v_O$
  然而，它有可能进入一个不稳定的平衡点，在该点上$v_I=v_O$

#### Six-Transistor (Six-T) Cell

- The cross-coupled inverter pair is the basic storage element. Each inverter has two transistors
  交叉耦合的反相器对是基本的存储元件。每个反相器有两个晶体管。
- Two additional transistors, $M_{A1}$ and $M_{A2}$ , are called **access transistors** or pass transistors. Their functions are
  两个额外的晶体管$M_{A1}$和$M_{A2}$被称为**访问晶体管**或传输晶体管。它们的功能是
	1. to isolate the cell from other cells
	   将本单元与其他单元隔离
	2. to provide a path for information to be written and read from the memory cell
	   为信息提供一个路径，以便从存储单元中读取和写入数据
- Data can be stored either as a **1** on point $D_1$ and **0** on point $D_2$ or vice-versa.
  数据可以存储为点$D_1$存储为**1**、点$D_2$存储为**0**，反之亦然

##### Commonly Used SRAM Memory Cells

![[Pasted image 20241105213354.png]]

- The advantage of the CMOS memory cell compared to others:
  CMOS存储器单元对比其他的优势有：
	- Small power dissipation.
	  更小的功耗
	- Small size.
	  小小的也很可爱
	- Small leakage current.
	  更小的漏电流

##### Read Operation of a 6-T Cell

###### Read 0

![[Pasted image 20241105214700.png#pic_center|]]

($0V@D_1$ and $3V@D_2$ for a $V_{DD}$ of $3V$)
1. With $\text{Wordline}(\text{WL})=0V$, the two bitlines for the cell are selected, and precharged to, say, $1.5V$.
   当$\text{字线}(\text{WL})=0V$时，单元的两个位线被选中，并预充电至例如1.5V。
2. The access transistors $M_{A1}$ and $M_{A2}$ are then turned **ON** (or **accessed**) by raising Wordline(WL) to $V_{DD}=3V$
   然后通过将字线(WL)提高到$(V_{DD}=3V)$，使访问晶体管$M_{A1}$和$M_{A2}$导通（访问）。
   Conditions prevailing at this time are as follows:
   ![[Pasted image 20241105220105.png#pic_center|]]
   此时的条件如下：
	- $M_{A1}$ is **ON**, Linear Region
	  $V_{GS}>V_T$ as $(3-0)>1$
	  $V_{DS}<V_{GS}-V_T$ as $(1.5-0)<(3-1)$
	- $M_{A2}$ is ON, Saturation
	  $V_{GS}>V_T$ as $(3-1.5)>1$
	  $V_{DS}>V_{GS}-V_T$ as $(3-1.5)>\left(\left(3-1.5\right)-1\right)$

###### Read 1