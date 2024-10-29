# Power Supply to a Passive Load

# Power Supply to a Active Load

# Power Supplies

## Linear

![[Linear Power Supply.png#pic_center|Linear Power Supply]]

- Step-down then rectified at power frequency and generates harmonics at multiples of 100 Hz (2 times 50 Hz for full-wave rectifier)
- These harmonics decay significantly after 10 kHz.
- Bulky transformer and significant power dissipation in the regulator results in poor conversion efficiency (20 to 40%).

## Switched Mode (SMPS)

![[Switch-Mode Power Supply.png#pic_center|Switch-Mode Power Supply]]

- Rectified then step-down cation through DC-DC conversion at 50-150 kHz switching frequency.
- Generate harmonics up to several tens of MHz.
- Compact transformer and excellent conversion efficiency (70 to 90%) but generate significant EMI.

# Conducted EMI Through Power Grid

- Practically all consumer electronics use **[[EMI Filter#Switched Mode (SMPS)|SMPS]]** due to its high conversion efficiency.
- SMPS is noisy and it poses an EMI threat to other sensitive equipment connected to the same power network.
- Suppression of conducted EMI from the SMPS is needed to meet EMC regulatory requirement.

## Measurement of Conducted EMI

### Current Probe

![[Pasted image 20241029193951.png#pic_center|Current Probe]]
- This is the most straight forward setup to measure RF interference current from the **equipment under test** (EUT).
- Unfortunately, the **repeatability** of the measurement is a big problem!

#### Example

A SMPS is powered by an AC power mains. It generates RF noise currents into the power mains through the power cord.

![[Pasted image 20241029201003.png#pic_center|]]

- The AC power mains can be modelled as a 50Hz AC source with a source resistance of $R_s$
- The SMPS can be modelled as a noise source $V_n$ with a source resistance of $R_n$

1. If $V_n=10mV$ and $R_n=30\mathrm{\Omega}$ at 1MHz, what is the expected level of RF noise current at 1MHz in the power line for $R_s=10\mathrm{\Omega}$?
2. If $R_s$ changes to $100\mathrm{\Omega}$, what is the expected level of RF noise current?

##### 解

- As we are only interested in RF noise current at 1 MHz, we could treat the 50Hz AC source as a short circuit for ease of analysis.
1. When $R_s=10\mathrm{\Omega}$, $$I_n=\frac{V_n}{R_n+R_s}=250\mathrm{\mu A}=48\mathrm{dB\mu A}$$
2. When $R_s=100\mathrm{\Omega}$, $$I_n=\frac{V_n}{R_n+R_s}=77\mathrm{\mu A}=37.7\mathrm{dB\mu A}$$

##### 结论

- The fluctuation of AC mains impedance $R_s$ causes large variation of RF noise current (almost $10\mathrm{dB}$), which results in repeatability of the RF noise current measurement!

### Line Impedance Stabilization Network (LISN)

- Measurement with repeatability
- A device called **Line Impedance Stabilization Network (LISN)** is inserted between the AC mains and the EUT to ensure repeatability of the conducted EMI measurement.
- Details of “LISN” can be found in IEC-CISPR 16-1 Standard: Radio disturbance and immunity measurement apparatus.

#### Work

![[Pasted image 20241029201807.png|LISN]]
- At the **power frequency (50Hz)**, the LISN is practically **transparent** to the AC power (230V, 50Hz) and the EUT receives the power.
- At the **EMI frequency (says, 5MHz)**, the high frequency noise current of the EUT will flow through C1 and measured by the $50\mathrm{\Omega}$ test instrument.