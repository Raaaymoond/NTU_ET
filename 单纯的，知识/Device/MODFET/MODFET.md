---
aliases: 
tags:
  - heterostructure
  - MODFET
---

- In a FET there is a gate-controlled channel through which current is allowed to flow.
- The gate must be isolated from the channel current flow. Otherwise, an input signal current, while on its way to the output, would “leak” through the gate, leading to a poor gain for the FET.
  栅极必须与沟道电流隔离。否则，输入信号电流在到达输出时会“泄漏”到栅极，导致FET增益变差。

## Two types of conventional FETs

![[MODFET_FIG1.png#pic_center|MOSFET]]
1. Metal Oxide Semiconductor FETs (MOSFETs)
	- The gate isolation is provided by depositing an oxide between the gate and the active channel.
	- **The n-channel is induced at the p-type $\mathrm{Si}$ surface due to strong inversion associated with band bending and controlled by gate voltage $V_{GS}$.**
	- The electron flow in the channel forms current $I_{DS}$ when $V_{GS}> V_T$ , and $V_{DS}>0$.
![[MODFET_FIG2.png#pic_center|MESFET]]
2. Metal Semiconductor FETs (MESFETs)
	- In a Metal Semiconductor FET (**no oxide**), the metal gate forms a [[Schottky Barrier]] with the semiconductor.
	- **The n-channel is a part of the n-type Si, which is not covered by the depletion region of the [[Schottky Barrier]], and controlled by the reverse-biased Shottky contact.**

## New FETs Developed Using Heterostructures

- Modulation-doped Field Effect Transistors (MODFETs)
- They are also called:
	- Heterostructure Insulated Gate FETs (HIGFETs)
	- High Electron Mobility Transistors (HEMTs)
	- Two-dimensional Electron Gas FETs (TEGFETs)

# Device Structures

![[MODFET_FIG3.png|A systematic of a GaAs/AlGaAs n-MODFET]]
1. Semi-Insulating GaAs Substrate.
   半绝缘GaAs
2. Undoped GaAs, 2-dimensional $e$ gas is formed on the surface of this layer.
   未掺杂的GaAs，这个区域会形成二维电子气
3. Undoped AlGaAs as a spacer which separates the electrons in undoped GaAs and the donor ions in doped AlGaAs.
   未掺杂的AlGaAs形成间隔层，将未掺杂GaAs层的电子和掺杂的AlGaAs层的施主离子隔离
4. Donor-doped AlGaAs.
   施主掺杂的AlGaAs
5. Metal gate which forms [[Schottky Barrier]] with the doped AlGaAs.
   金属栅极，与掺杂的AlGaAs形成肖特基势垒

The energy band profile shows band bending leading to a triangular quantum well at the $\mathrm{GaAs/AlGaAs}$ interface. 
![[MODFET_FIG4.png#pic_center|]]
# Modulation Doping

![[MODFET_FIG5.png#pic_center|]]
![[MODFET_FIG6.png#pic_center|]]

- The doped wide bandgap $n^+$ AlGaAs has donor ions and electrons.
  宽带隙的$n^+$ AlGaAs有施主离子和电子
- The electrons could transfer through the undoped AlGaAs spacer to the narrow bandgap undoped GaAs as it has lower energy states for electrons.
  电子穿过未掺杂的AlGaAs隔离层到窄带隙的GaAs，因为GaAs层的电子能级更小
- The positively charged donor ions and the negatively charged electrons are then spatially separated by the undoped AlGaAs spacer.
  正电荷施主离子和负电荷电子被未掺杂的AlGaAs层上在空间上分开
- The dipole effect produces band bending.
  偶极效应导致能带弯曲
- The energy states in undoped GaAs are quantized, $E_1$ is the ground level.
  未掺杂GaAs中能级是量子化的，$E_1$是基态

## Advantages of the Modulation Doping

- Because the electrons at the surface of the narrow gap GaAs are spatially separated from the positively charged dopant ions by the undoped AlGaAs spacer, these electrons are virtually free to move in the undoped GaAs channel and essentially remain free from impurity ion scattering. **Thus, they have high mobility**.
  由于在窄带隙GaAs表面的电子从空间上与带正电的杂质离子被未掺杂的AlGaAs隔离层隔离，这些电子在未掺杂的GaAs沟道中几乎可以自由移动，并且基本上不受杂质离子散射的影响。**因此，它们具有高迁移率**。
  ![[MODFET_FIG7.png#pic_center|2-dimensional property]]
- As the trapped electrons have 2-dimensional properties (moving in x-y plane), hence they are called two-dimensional electron gas. The sheet electron concentration is very high as they are limited to a very thin surface layer of the GaAs.
  由于被捕获的电子具有二维特性（在x-y平面内移动），因此它们被称为二维电子气。面电子浓度非常高，因为它们被限制在非常薄的GaAs的表面层。

![[MODFET_FIG8.png#pic_center]]

- The two-dimensional electron gas has the highest mobility at a **given temperature**. 
- This is why such devices are also called **High Electron Mobility Transistors (HEMTs)**.

# Normally-off and normally-on Devices

- To control the drain-source current $I_D$ by means of a gate voltage $V_G$, the thickness of the wide bandgap layer between the gate metal and the 2DEG is critical.
- By varying the thickness of the wide-bandgap layer, the MODFET can be made either a normally off (enhancement mode) or normally on (depletion mode) device.

## Normally-off or Enhancement-mode MODFETs

- When the wide-bandgap layer is thin, the MODFET will be a normally-off device.
![[Pasted image 20241102014640.png]]
- Energy band diagrams of a normally-off MODFET at
	- (a) [[Thermal Equilibrium]]
	- (b) The onset of threshold ($V_T>0$)
- $d_1$ and $d_0$ are the thicknesses of the doped and undoped regions of the wide bandgap semiconductor, respectively
- $\Delta E_C$ is the conduction bandgap offset

- For small AlGaAs thickness, the gate [[Schottky Barrier]] can completely deplete the electrons in the AlGaAs as well as the 2DEG even at zero gate bias, thus leading to enhancement-mode type or normally off devices.
  AlGaAs厚度较小的情况下，即使没有栅极偏置，栅极的肖特基势垒也可以完全耗尽AlGaAs和二位电子气中的电子，从而获得了增强型或者常闭型器件。![[MODFET_FIG9.png#pic_center|Depletion Width of Schottky Contact]]
  The depletion width of the Schottky contact $W$ is greater than $d_1+d_0$. No channel is formed at the narrow bandgap GaAs surface.
- A **positive gate** voltage (greater than the threshold voltage $V_T$) is required to turn the device on. When $V_G=V_T$ , the depletion width $W=d_1+d_0$ ![[Pasted image 20241102024935.png#pic_center]] The threshold voltage can be adjusted by control of AlGaAs thickness and doping. $$V_T=\phi_{Bn}-\frac{\Delta E_C}{q}-V_p$$ Where ^9de4ef
	- $\phi_{Bn}$ is the barrier height
	- $V_p$ is a pinch-off voltage of the n-type AlGaAs $$V_p=\frac{q}{\epsilon_s}\int_0^d N_D(x)x\mathrm{d}x=\frac{qN_Dd_1^2}{2\epsilon_s}$$ Where ^9bdcde
		- $\epsilon_s$ is the permittivity of the AlGaAs materials
		- $N_D$ is the doping concentration
- When the gate voltage is larger than $V_T$, a charge sheet will be capacitively induced by the gate at the heterojunction interface. ![[Pasted image 20241102025701.png#pic_center|]] The sheet carrier concentration (**number of the carriers per unit area**) is defined as $$n_s(y)=\frac{C_g\left(V_G-V_T-V(y)\right)}{q}$$ Where
	- $y$ is zero at the source and $L$ at the drain
	- $V(y)$ is the voltage at position $y$ due to drain voltage
	- $C_g$ is the deleption capacitance per unit area $$C_g=\frac{\epsilon_s}{d_1+d_0+\Delta d}$$ Where
		- $\Delta d$ is a correction factor (some authors take $\Delta d$ as the thickness of channel or inversion layer) $$\Delta d=\frac{\epsilon_s\cdot a}{q}\approx8\mathrm{nm}$$

## Normally-on or Depletion-mode MODFETs

- When the wide bandgap layer is thick enough, the MODFETs will be Normally-on or Depletion-mode devices.
- For thicker AlGaAs layers, the depletion region of the [[Schottky Barrier]] does not deplete the electron gas at zero gate voltage ($W<d=d_1+d_0$). Such devices are Normally-on or Depletion-mode devices. (A channel exists at $V_G=0$). ![[Pasted image 20241102030333.png#pic_center|]]

- A negative gate voltage is required to deplete the electron gas and pinch the device off. ($V_T<0$) ![[Pasted image 20241102030724.png#pic_center]]

## Example

Consider an AlGaAs/GaAs heterojunction with n-AlGaAs doped to $2\times 10^{18} cm^{-3}$ and a thickness of $40\mathrm{nm}$. Assume the undoped spacer layer is $3\mathrm{nm}$ and the Schottky barrier height is $0.85e\mathrm{V}$ and $\Delta E_C/q=0.23\mathrm{V}$. The dielectric constant of the AlGaAs is 12.3. Calculate the two-dimensional electron gas concentration for such heterojunction at $V_G=0$.

### Solution

- 首先判断器件类型（常开还是常闭），判断依据是[[MODFET#^9de4ef|阈值电压]]$V_T$ $$V_T=\phi_{Bn}-\frac{\Delta E_C}{q}-V_p$$
	- 肖特基势垒$q\phi_{Bn}=0.85e\mathrm{V}\implies \phi_{Bn}=0.85V$
	- $\frac{\Delta E_C}{q}=0.23V$
	- [[MODFET#^9bdcde|pinch-off voltage]]: $$V_p=\frac{qN_Dd_1^2}{2\epsilon_s}$$
		- 掺杂浓度$N_D=2\times 10^{18}\mathrm{cm}^{-3}$
		- AlGaAs厚度$d_1=40\mathrm{nm}=40\times10^{-7}\mathrm{cm}$
		- 相对介电常数$\epsilon_s=12.3$，所以介电常数为$\epsilon_s\cdot\epsilon_0$
		$$\implies V_p=2.35\mathrm{V}$$
	所以阈值电压$V_T$：$$V_T=0.85-0.23-2.35=-1.73\mathrm{V}$$
- 二维电子气浓度$n_s$： $$n_s=\frac{\epsilon_s\epsilon_0}{d_1+d_0+\Delta d}\frac{V_G-V_T}{q}=2.30\times 10^{12}cm^{-2}$$

# Current-Voltage Characteristics

- The current voltage characteristics of a MODFET can be obtained in the way similar to the MOSFET. The current at any point along the channel is $$I_D=Wq\mu_n n_s\xi_y=W\mu_nC_g\left[V_G-V_T-V(y)\right]\frac{\mathrm{d}V(y)}{\mathrm{d}y}$$ Where:
	- $W$ is the channel width
	- $\xi_y$ is longitudinal electric field
- Since the current is constant along the channel, integrating the equation from source to drain ($y=0$ to $y=L$) gives $$I_D=\frac{W}{L}\mu_n C_g\left[(V_G-V_T)V_D-\frac{V_D^2}{2}\right]$$
	- When $V_D\ll(V_G-V_T)$, it is in linear region and $$I_D=\frac{W}{L}\mu_nC_g\left[(V_G-V_T)V_D\right]$$
	- At large drain voltage, the charge sheet $n_s(y)$ at the drain is reduced to 0. So $V_{Dsat}=V_G-V_T$ and the saturation current is $$I_{Dsat}=\frac{W\mu_nC_g}{2L}\left(V_G-V_T\right)^2=\frac{W\mu_n\epsilon_s}{2L(d_1+d_0+\Delta d)}(V_G-V_T)^2$$
	- For high-speed operations, the longitudinal field along the channel is sufficiently high to cause carrier drift velocity saturation ($v_{ds}$). The current (maximum) in the velocity-saturation region is $$I_{Dmax}=qn_sv_{ds}W=C_g(V_G-V_T)v_{ds}W$$
# Important Parameters

## Channel Conductance

$$g_d=\frac{\partial I_D}{\partial V_D}\Bigg|_{V_G}$$
The electron draft velocity is $v_d=\mu\xi$
where:
- $\mu$ is [[Carrier Mobility]]
- $\xi$ is electric field and $\xi=\frac{V_D}{L}$ , $L$ is channel length

$$\displaylines{I_D=q n_s v_d W=Wq n_s\mu_n\xi_y=\frac{W}{L}V_D q n_s \mu_n\\\implies g_d=\frac{W}{L}q n_s \mu_n}$$

With $n_s=10^{12}\mathrm{cm^{-2}}$ in a channel $1\mu\mathrm{m}$ long and $10\mu\mathrm{m}$ wide, and $\mu_n$ of electrons in the GaAs channel is $7000cm^2\cdot V^{-1}s^{-1}$, then $g_d=1.12\times 10^{-2}\mathrm{S(siemens)}$, which is **10 times higher** than in a Si MOSFET.

## Transconductance

$$g_m=\frac{\partial I_D}{\partial V_G}\Bigg|_{V_D}\implies g_m(\mathrm{sat})=\frac{\partial}{\partial V_G}C_g v_{ds}W(V_G-V_T)=C_g v_{ds}W$$
- 其中$v_{ds}$是速度饱和的速度

## Transit Time

$$t_r=\frac{L}{v_{ds}}$$
For $L=1\mu\mathrm{m}$ and $v_{ds}=2\times 10^7\mathrm{cm\cdot s^{-1}}$, the transit time is $5\mathrm{ps}$.

MODFETs have very small transit time that enables them to be used as high-speed devices.
# Cutoff Frequency

- The speed of a MODFET is measured by the cutoff frequency $$f_T=\frac{g_m}{2\pi(\mathrm{total\ capacitance})}=\frac{W v_{ds} C_g}{2\pi (WL C_g+C_p)}$$ where:
	- $C_p$ is the parasitic capacitance
- To improve $f_T$, we should consider a semiconductor with large $v_{ds}$, a gate structure with an ultra short gate length, and a device configuration with minimum parasitic capacitance.

## Cutoff Frequency Versus Channel or Gate Length for Five Kinds of Field-Effect Transistors

![[Pasted image 20241102041324.png]]
- The best pseudomorphic SiGe MODFETs have a $f_T$ comparable to the GaAs MODFET. SiGe MODFETs are attractive because they can be processed with silicon fabrication facilities.
- The $\mathrm{Al_{0.48}In_{0.52}As-Ga_{0.47}In_{0.53}As}$ MODFET formed on a InP substrate has higher $f_T$, mainly due to the high electron mobility and velocities in the $\mathrm{Ga_{0.47}In_{0.53}As}$. The $f_T$ at a gate length of $50\mathrm{nm}$ can be as high as $600\mathrm{GHz}$.

# Summary

- The MODFET is a device which enhanced high-frequency performance. This device structure is similar to that of a MESFET except there is a heterojunction under the gate. A two-dimensional electron gas, i.e., a conductive channel, is formed at the heterojunction interface, and electrons with high mobility and high average drift velocity can be transported from the source through the channel to the drain.
  MODFET是一种增强高频性能的器件。其结构类似于MESFET，但在栅极下方有异质结。在异质结界面形成了二维电子气，即导电沟道，具有高迁移率和高平均漂移速度的电子可以从源极通过沟道到达漏极。
- The output characteristics of all field-effect transistors (FETs) are similar. They all have a linear region at low-drain biases. As the bias increases, the output current eventually saturates, and at a sufficiently high voltage, avalanche breakdown occurs at the drain. Depending on whether it requires a positive- or negative-threshold voltage, FET can be either normally off (enhancement mode) or normally on (depletion mode).
  所有场效应晶体管（FET）的输出特性都相似。它们在低漏极偏置时都有一个线性区域。随着偏置的增加，输出电流最终会饱和，并且在足够高的电压下，会在漏极处发生雪崩击穿。根据是否需要正阈值电压或负阈值电压，FET可以是常断型（增强模式）或常通型（耗尽模式）。
- The cutoff frequency $f_T$ is a figure of merit for the high-frequency performance of a FET. The conventional GaAs MODFET and the pseudomorphic SiGe MODFET have a $f_T$ about 30% higher than that of the GaAs MESFET. The GaInAs MODFET has the highest $f_T$ and it has a projected $f_T$ of $600\mathrm{GHz}$ at a gate length of $50\mathrm{nm}$.
  截止频率$f_T$是评估 FET 高频性能的指标。传统的 GaAs MODFET 和伪SiGe MODFET 的$f_T$大约比GaAs MESFET高30%.GaInAs MODFET具有最高的$f_T$,在$50\mathrm{nm}$栅极长度下的$f_T$为$600\mathrm{GHz}$。