---
aliases: 
tags:
  - heterostructure
---

# Semiconductor Lasers

## Photon-electron Interaction

There are three processes for interaction between a photon and an electron in a solid:
- absorption
- spontaneous emission
- stimulated emission

### Absorption

If an atom in state $E_1$ absorbs the photon, it goes to the excited state $E_2$. The change in the energy state is the **absorption process**. The requirement is $hf_{12}=E_2-E_1$.
如果处于状态$E_1$的原子吸收光子，它会进入激发态$E_2$。能级变化的过程称为**吸收**。要求是$hf_{12}=E_2-E_1$。

### Spontaneous Emission

The excited state of the atom is unstable. Without any external stimulus, the atom can make a transition to the ground state, giving off a photon of energy $hf_{12}$. This process is called **spontaneous emission**. Thus, $E_2-E_1=hf_{12}$.
原子的激发态是不稳定的。在没有任何外部刺激的情况下，原子可以跃迁到基态，并发出能量为$hf_{12}$的光子。这个过程称为**自发辐射**。因此，$E_2-E_1=hf_{12}$。

### Stimulates Emission

When a photon of energy $hf_{12}$ impinges on an atom while it is in the excited state, the atom can be stimulated to make a transition to the ground state and gives off a photon of energy $hf_{12}$. This process is called **stimulated emission**.
当能量为 $hf_{12}$ 的光子撞击处于激发态的原子时，原子可以被刺激到跃迁到基态，并发出一个能量为 $hf_{12}$ 的光子。这个过程被称为**受激发射**。
The radiation from stimualted emission if **coherent** because all photons emitted are in phase (the same energy and wave vector).
受激发射产生的辐射是**相干的**，因为所有发射的光子都是同相的（具有相同的能量和波矢）。

## Dominant Interaction Process In Devices

- LEDs: Spontaneous Emission
- Laser Diodes: Stimulated Emission
- Photodetectors and Solar Cells: Absorption

## Semiconductor Materials for Lasers

- All lasing semiconductors must have **direct bandgaps** because of the momentum conservation and high radiative-transition probability.
  所有激光半导体必须具有**直接带隙**，因为需要满足动量守恒和高辐射跃迁几率。
- The laser emission wavelengths range: $0.3$ to $30\mu\mathrm{m}$.
- GaAs was the first material to emit laser radiation and its related III-V compound alloys are extensively studied.
- Three most important III-V compound alloy systems for lasers are:
	- GaInAsP
	- GaInAsSb
	- AlGaAsSb

## Features of Semiconductor Lasers

- Similar to the solid-state ruby laser and helium-neon gas laser, semiconductor lasers are highly monochromatic and can produce a highly directional beam of light.
  与固态红宝石激光器和氦氖气体激光器相似，半导体激光器也是高度单色的，并且可以产生高度定向的光束。
- Differ from other lasers, semiconductor lasers are small (about 0.1 mm long) and can be easily modulated at high frequencies by simply modulating the biasing current.
  不同于其他激光器，半导体激光器体积小（约0.1毫米长），并且可以通过简单调节偏置电流高频调制。
- They are the important light source for optical communication, video recording, optical reading, high speeding printing.
  它们是光通信、视频录制、光学读取和高速打印的重要光源。

# Laser Operation

- Three conditions for laser operation:
	- [[Population Inversion]]
	  粒子数分布反转
	- [[Carrier and Optical Confinements]]
	  载流子和光学限制
	- [[Optical Cavity]]
	  光学谐振腔

# DH Laser

The energy diagram of a DH lasers made of GaAs/AlGaAs
![[Pasted image 20241103040341.png#pic_center]]
- The stimulated emission is from the GaAs, and the emission frequency $\nu$ is such that $h\nu=E_g(\mathrm{GaAs})$. The corresponding wavelength$$\lambda(\mu \mathrm{m})=1.24/E_g(e\mathrm{V})=0.880\mu \mathrm{m}$$
  受激发射源于GaAs，其发射频率$\nu$满足$h\nu=E_g(\mathrm{GaAs})$。
- To achieve tuning wavelength of laser, an AlGaAs layer should be the active layer instead of GaAs. But the bandgap of the AlGaAs active layer must be less than that of the p-AlGaAs and n-AlGaAs barrier layers.
  为了实现激光波长可调，有源层应该使用AlGaAs而不是GaAs。但AlGaAs有源层的带隙必须小于p-AlGaAs和n-AlGaAs势垒层的带隙。

## Threshold Current and Threshold Current Density

- The threshold current is the minimum current required for lasing to occur.
- The current upto threshold is given by the usual forward biased [[Diode I-V Relation|p-n junction current equation]].
  小于阈值电流的电流表达式由普通的正向偏置 p-n 结电流方程给出。$$I=I_o\left(e^{\frac{V_A-IR_S}{V_T}}-1\right)$$Where: ^52252a
	- $V_A$ is the applied voltage
	- $I_o$ is the saturation current at the operating temperature $T(K)$
- Once laser action starts above the threshold, then the junction voltage drop is $\frac{E_g}{q}$ , where $E_g$ is the active layer bandgap. The current now will be
  一旦激光作用超过阈值，结电压降为 $\frac{E_g}{q}$，其中 $E_g$ 是有源层的带隙。此时的电流将会是$$I=\frac{V_A-E_g/q}{R_S}$$ ^9ec28f
- The threshold current density can be expressed as$$J_{\mathrm{threshold}}=\frac{1}{\beta}\left[\alpha+\frac{1}{2L}\mathrm{ln}\left(\frac{1}{R_1R_2}\right)\right]$$where:
	- $\beta$ is the **gain factor**
	- $\alpha$ is the loss per unit length from absorption and other scattering mechanism
	- $L$ is the cavity length
	- $R$ is the reflectance of the cavity$$R=\left(\frac{n-1}{n+1}\right)^2$$
  $J_{\mathrm{threshold}}$ may be different in different book

## Threshold Current Varies With Temperature

![[Pasted image 20241103044849.png]]

- (a) Light Output versus Diode Current for a GaAs/AlGaAs DH laser.
	- the output power becomes lower at high temperature
	- $I_{\mathrm{threshold}}$ increases with temperature
- (b) Temperature Dependence of the Continuous-Wave Current Threshold.
	- $I_{\mathrm{threshold}}$ follows an exponential relation with temperature,$$I_{\mathrm{threshold}}=I_o e^{\frac{T}{T_o}}$$where:
		- $I_o$ is a **constant**, dependent on device type and size
		- $T_o$ is called **characteristic temperature**, 110 Celsius for this laser

## Example

A double heterojunction laser diode is connected in a closed circuit with a series resistor and a variable power supply. The device shows no emission at a bias of 2V and an injected current of 0.9A but strong emission at a bias of 5.7V and a current of 2A. Assume that the device operates at room temperature and has a saturation current of 0.1A.

### Solution

由于在室温（300K），所以[[Thermal Voltage|热电压]]为$V_T=26m\mathrm{V}$

饱和电流$I_S=0.1\mathrm{A}$

在2V正向电压时没有发射，在此时套用[[Heterojunction Photonic (Optoelectronic)  Devices#^52252a|普通的pn结电流公式]]：$$I=I_S\left(e^\frac{V_F-IR_S}{V_T}-1\right)$$
（呃啊我草泥马不要什么地方都把pn结公式里的减1省掉啊草泥马）

代入饱和电流和热电压可以解得$$R_S=2.16\Omega$$

代入[[Heterojunction Photonic (Optoelectronic)  Devices#^9ec28f|发射时的电流公式]]求带隙：$$I=\frac{V_A-E_g/q}{R_S}\implies E_g=1.38e\mathrm{V}$$（这里的单位选择电子伏特会比较好算）

算波长$$\lambda=\frac{ch}{E_g}=900\mathrm{nm}$$
上式中：
- $c$为光速
- $h$为普朗克常数

# Quantum Well Lasers

