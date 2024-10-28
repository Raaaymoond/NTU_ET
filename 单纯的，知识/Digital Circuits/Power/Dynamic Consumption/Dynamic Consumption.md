---
aliases:
  - Dynamic Dissipation
tags:
  - digital_circuits
  - power
---
# Goh

- Dynamic power is required to charge & discharge load capacitances when transistors switch.
- One cycle involves a rising and falling output.
- On rising output, charge $Q = CV_{DD}$ is required
- On falling output, charge is dumped to GND
- This repeats $Tf_{sw}$ times over an interval of $T$
- $P_{\mathrm{dynamic}}=C_L V_{DD}^2 f_{sw}$, $f_{sw}=\alpha f$, 其中$f$为时钟频率，$\alpha$为[[Switching Activity]]

# Gwee

- When the capacitor $C_L$ gets charged through the pMOS transistor, its voltage rises from 0 to Vdd, and a certain amount of energy ($C_LV_{DD}^2$) is drawn from the power supply. Part of this energy ($1/2 C_LV_{DD}^2$) is dissipated in the pMOS device, while the remainder is stored on the load capacitance. During the high-to-low transition, this capacitor is discharged, and the stored energy is dissipated in the nMOS transistor
- Each switching cycle (consisting of an $L\to H$ and an $H\to L$ transition) takes a fixed amount of energy, equal to $C_LV_{DD}^2$
- Power consumption is dependent on how often the device is switched. If the gate is switched on and off f times per second, the power consumption equals $P_{\mathrm{dynamic}}=f C_LV_{DD}^2$
	- Actual activity is somewhat lower as not all gates in the complete IC switch at the full rate of $f\mathrm{MHz}$ and this is accomodated by replacing $C_L$ by $C_{EFF}=\widehat{C_L}$ where $C_{EFF}$ (effective capacitance) is the average capacitance switched every clock cycle and $\widehat{P_{0\to 1}}$ is the activity factor.

# Ivan

- In CMOS designs, power consumption is a function of power supply ($V_{DD}$), operating frequency ($f$), total load capacitance ($C_L$) and switching activity ($\alpha$). $$P=f\times C_L \times V_{DD}^2 \times \sum\alpha$$
- It can be seen from the equation that reducing  leads to quadratic power savings.
- However, reducing $V_{DD}$ also leads to delay increasing and loss of performance.
- 