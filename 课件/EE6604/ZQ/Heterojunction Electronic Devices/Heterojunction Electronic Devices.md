---
aliases: 
tags:
  - semi_conductor
  - heterostructure
---

# Fundamentals

- [[Heterojunction]]

## Material Parameters of Alloy Semiconductors

- An **alloy semiconductor is a combination of two or more semiconductors**, elemental semiconductors ($\mathrm{Si}$ with $\mathrm{Ge}$) or semiconductor compound from the same group ($\mathrm{GaAs}$ with $\mathrm{InAs}$ or $\mathrm{ZnS}$ with $\mathrm{ZnSe}$).
- An alloy is formed from a physical mixture of two or more compounds, while a compound is formed from a chemical reaction. $\mathrm{GaAs}$ (or $\mathrm{InAs}$) is a compound semiconductor.
- $\mathrm{Ga_{1−x} In_x As}$ is an alloy compound consisting of $\mathrm{GaAs}$ and $\mathrm{InAs}$ with a mole ratio of $(1−x):x$.
- **Alloy semiconductors** could be binary ($\mathrm{SiGe}$, $\mathrm{GaAs}$, $\mathrm{InP}$), or ternary ($\mathrm{Al_x Ga_{1-x} As}$, $\mathrm{In_x Al_{1-x} As}$), or quaternary ($\mathrm{In_x Ga_{1-x} As_y P_{1-y}}$).
- The material parameters include energy bandgap, lattice constant, thermal conductivity, melting point, etc. The first two, **[[Heterojunction Electronic Devices#energy bandgap|Energy Bandgap]]** and **[[Lattice Constant]]** are the most important ones.

#### Vegard's Law

- [[Vegard’s Law]]

### Lattice Constant

- [[Lattice Constant]]

#### Lattice Constant Variation as a Function of [[Vegard’s Law#^648b21|Mole Fraction]]

![[Lattice Constant Variation as a Function of Mole Fraction.png#pic_center]]

### Energy Bandgap

- The bandgaps of the [[Vegard’s Law#Ternary Compound|Ternary Compound]] and [[Vegard’s Law#Quaternary Compound|Quaternary Compound]] semiconductors only approximately follow Vegard’s Law. $$E_g(A_xB_{1-x}C)=xE_g(AC)+(1-x)E_g(BC)$$
- In most alloys, there is a **bowing effect** arising from the increasing disorder due to alloying of different elements. The energy bandgap of alloy semiconductors can bebetter described by the following expression: $$E_g(\mathrm{alloy})=a+bx+cx^2$$

![[Compositional Dependence of Energy Bandgap.png#pic_center|Compositional Dependence of Energy Bandgap of the III-V Alloys at 300 K]]

## Lattice Match and Mismatch Heterostructures

- There are two kinds of heterostructures:
	- **[[Lattice-Matched Heterostructures]]**
	- **[[Lattice-Mismatched Heterostructures]]**
		- The **lattice-mismatched heterostructures** can be further classified as **Strained Heterostructure** and **Unstrained Heterostructure**.

![[Lattice Match and Mismatch Heterostructures.png#pic_center|Lattice Match and Mismatch Heterostructures]]

### Critical Thickness

- [[Critical Thickness]]

![[Critical thickness vs. Mismatch for Si Substrate.png#pic_center|Critical thickness vs. Mismatch for Si Substrate]]
- A greater mismatch corresponds to a smaller critical thickness
- A smaller mismatch corresponds to a greater critical thickness

## Bandgap Discontinuity

^4ac8f1

- Two materials have different energy bandgaps. There are possibly three types of band-edge lineups:
	- Straddling
	- Staggered
	- Broken Gap
- Each of these has unique and special band structure and device applications.

### Straddling Bandgap

![[Straddling.png#pic_center|Straddling]]

### Staggered Bandgap

![[Staggered.png#pic_center|Staggered]]

### Broken Gap

![[Broken Gap.png#pic_center|Broken Gap]]

## The Band Diagram for Heterostructures

![[Energy band diagrams for nonuniform band structure and doping.png|Energy band diagrams for nonuniform band structure and doping. (a) before contact; (b) after contacted.]]

- Consider the energy band diagrams for two materials with different [[Electron Affinity]] $\mathrm{q}\chi$ , the energy gaps $E_g=E_c-E_v$ and the chemical potentials or [[Fermi Level|Fermi Energy]] $E_f$.
- Note:
	- [[Vacuum Level]] must be continuous
	- The band bending upward means an increase in electron energy, decrease in electron density
	- The band bending downward means a decrease in electron energy, increase in electron density

### Bandgap Offset

![[Bandgap Offset.png|Bandgap Offset]]

$$\displaylines{
\Delta E =& E_{g1}-E_{g2}=\Delta E_C+\Delta E_V \\
\Delta E_C =& E_{C1}-E_{C2} \\
\Delta E_V =& E_{V2}-E_{V1}
}$$
- The ratio $\Delta E_C/\Delta E_V$ varies with material systems and is not easy to be determined.
- The $\mathrm{GaAs/AlAs}$ and $\mathrm{GaAs/AlGaAs}$ systems have type I structure, and the ratio $\Delta E_C/\Delta E_V$ is about 60:40.

- The band diagram of Metal/AlGaAs/GaAs [[Heterojunction|Heterostructure]] under [[Thermal Equilibrium]]
![[Pasted image 20241030020138.png#pic_center|The band diagram of Metal/AlGaAs/GaAs Heterostructure]]
# Heterojunction Bipolar Transistors (HBTs)

The bandgap of a [[Vegard’s Law#Ternary Alloys|Ternary Alloys]] or quaternary alloy semiconductor can be varied, by simply adjusting the composition $x$ or $y$.

The heterostructures formed by alloy semiconductors, therefore, have immense applications in various fields.

## Limitations of Homojunction BJTs

![[Carrier Distribution.png|Carrier Distribution]]

- The [[Emitter Injection Efficiency]] $\gamma$ is: $$\gamma=\frac{I_{En}}{I_{En}+I_{Ep}}$$ since $I_{Ep} \ll E_{En}$, if follows: $$\gamma=1-\frac{p_{E0}D_E W_{bn}}{n_{B0}D_BL_E}$$ where,
	- $p_{E0}$: Equilibrium hole concentration in the emitter
	- $n_{B0}$: Equilibrium electron concentration in the base
	- $W_{bn}$: Neutral width of the base
	- $D_E$, $D_B$: Diffusion coefficients of minority carriers in emitter and base respectively
	- $L_E$: Diffusion length of minority carriers in the emitter
- The [[Base Transport Factor]] $\alpha_T$ is: $$\alpha_T=\frac{I_{Cn}}{I_{En}}\approx \frac{I_C}{I_{En}}=1-\frac{W_{bn}^2}{2L_B^2}$$ where, 
	- $L_B$: The diffusion length of minority carriers in the base
- The [[Common Base Current Gain]] $\alpha_0$ is: $$\alpha_0=\frac{I_C}{I_E}=\frac{I_C}{I_{En}}\cdot \frac{I_{En}}{I_E}=\alpha_T\cdot \gamma$$ Substituting the expressions for $\alpha_T$ and $\gamma$, we get $$\alpha_0=\left[1-\frac{W_{bn}^2}{2L_B^2}\right]\cdot \left[1-\frac{p_{E0}D_E W_{bn}}{n_{B0}D_B L_E}\right]$$
- The [[Common Emitter Current Gain]] $\beta_0$ is: $$\beta_0=\frac{\alpha_0}{1-\alpha_0}\approx\frac{n_{B0}D_B L_E}{p_{E0}D_EW_{bn}}$$ To achieve a high $\beta_0$, 
	- $p_{E0} \ll n_{B0} \implies n_{E0} \gg p_{B0}$
	- $W_{bn}$ is very small, and $W_{bn} \ll L_B$
  These mean
	- Emitter doping should be very high and base doping should be relatively much lower.
	- The base should be very narrow.
### Limitations

- Too narrow and lightly doped base will result in
	- Large base resistance
	- Smaller breakdown voltage
- Too heavy doping in emitter will cause bandgap of emitter to shrink.

It will then cause the base injection to increase, emitter injection to decrease and eventually leading to decrease in the emitter efficiency and current gain.

#### Effect of Emitter Doping

The bandgap shrinkage caused by heavy doping in the n-type emitter results in a higher barrier for electron injection and lower barrier for hole injection ^099bec

![[Pasted image 20241101015806.png]]

In Si, the bandgap shrinkage due to doping is approximately given by $$\Delta E_g=-22.5\left(\frac{N_d}{10^{18}}\cdot\frac{300}{T}\right)^{1/2}(meV)$$
and the [[Common Emitter Current Gain]] becomes $$\beta\approx \beta_0 exp(-\frac{\left|\Delta E_g\right|}{kT})$$ decreasing with heavy doping.

Thereffore, with a simple n-p homojunction for the emitter-base, the performance of the npn BJT is limited.

## Remedy

- Use a large bandgap material for n-type emitter. The deivce will then become a heterojunction bipolar transistor (HBT)
- The main advantage of HBT is the high emitter efficiency
- HBTs also have high speed and high frequency capability in circuit operation

![[A HBT with an n-AlGaAs emitter and a p-GaAs base transistor.png|A HBT with an n-AlGaAs emitter and a p-GaAs base transistor (a) Device structure, (b) Band diagram at thermal equilibrium]]

### Common Emitter Current Gain of HBTs

- From the definition, $$\beta_0\approx\frac{n_{B0}D_B L_E}{p_{E0}D_E W_{bn}}$$ and from [[PN Product#Law of Mass Action|Law of Mass Action]], $np=n_i^2$, the minority carrier concentration in the emitter $p_{E0}$, is $$p_{E0}=\frac{n_o^2(\mathrm{emitter})}{N_E(\mathrm{emitter})}=\frac{N_CN_V exp(-\frac{E_{gE}}{kT})}{N_E}$$ where,
	- $N_C$: [[Effective Density of States]] in the conduction band
	- $N_V$: Effective Density of States in the valence band
	- $E_{gE}$ is the bandgap of the emitter
- The minority carrier concentration in the base $n_{B0}$ is $$n_{B0}=\frac{n_i^2(\mathrm{base})}{N_B(\mathrm{base})}=\frac{N_C^\prime N_V^\prime exp(-\frac{E_{gB}}{kT})}{N_B}$$ where, 
	- $N_C^\prime$ and $N_V^\prime$: [[Effective Density of States]] in conduction band and valence band respectively
	- $E_{gB}$: bandgap of base

Hence $$\displaylines{\beta_0=\frac{n_{B0}D_B L_E}{p_{E0} D_E W_{bn}}\approx \frac{N_E D_B L_E}{N_B D_E W_{bn}}exp(\frac{E_{gE}-E_{gB}}{kT})\\=\frac{N_E D_B L_E}{N_B D_E W_{bn}}exp(\frac{\Delta E_g}{kT})}$$

![[Pasted image 20241101033813.png#pic_center|]]
- Note that even if the base is heavily doped, the barrier for hole injection will be very high due to the large $\Delta E_V$ of E-B junction.
	- This means that one can dope the base heavily and achieve low base resistance.
	- One can also make the base narrower to achieve high speed.
	- Thus, all our requirements for a good performance transistor can be met by having a larger band gap emitter.

### Further Description

The superior performance of the HBT results directly from the valence-band discontinuity $\Delta E_V$ at the heterointerface (E-B junction). $\Delta E_V$ increases the **valence band barrier height** in the E-B heterojunction and thus **reduces the injection of holes from the base to the emitter**.

- This effect in the HBT allows the use of a heavily doped base while maintaining a high emitter efficiency and current gain. The heavily doped base can reduce the base sheet resistance. In addition, the base can be made very thin without concern about the punch-through effect in the narrow base region.
  这个效应使得异质结双极性晶体管（HBT）在使用重掺杂基区的同时保持高发射效率和电流增益。重掺杂基区可以降低基区电阻。此外，可以将基区做得非常薄，而不必担心在窄基区中发生击穿。
- A thin base region is desirable because it reduces the base transit time and enhances the cutoff frequency.
  薄基区是可取的，因为它减少了基区的渡越时间并提高了截止频率。

### Example

A HBT has a bandgap of $1.62eV$ for the emitter, and a $1.42eV$ for the base. A BJT has a bandgap of $1.42eV$ for both the emitter and base materials. It has an emitter doping of $10^{18}cm^{-3}$ and a base doping of $10^{15}cm^{-3}$.
1. If the HBT has the same doping as the BJT, find the improvement of $\beta_0$.
2. If the HBT has the same emitter doping and the same $\beta_0$ as the BJT, how much can we increase the base doping of the HBT? Assume that all other device parameters are the same.

#### Solution

1. 列出本征共射电流增益$\beta_0$的公式：$$\beta_0\approx \frac{N_E D_B L_E}{N_B D_E W_{bn}}exp\left(\frac{E_{gE}-E_{gB}}{kT}\right)$$ 在本题中HBT和BJT有着相同的掺杂浓度，所以可以得出：
	- $N_E(HBT)=N_E(BJT)$
	- $N_B(HBT)=N_B(BJT)$
	- 假设$D_B$、$D_E$、$L_E$、$W_{bn}$也是相同的（这也没说啊）
	- $\Delta E_g(HBT)=1.62-1.42=0.2eV$
	- $\Delta E_g(BJT)=0eV$
	所以可以得出：$$\displaylines{\frac{\beta_0(HBT)}{\beta_0(BJT)}=\frac{exp\left(\Delta Eg(HBT)/kT\right)}{exp(\Delta E_g(BJT))}=exp(\Delta E_g(HBT)/kT)\\=e^{0.2eV/0.0259eV}=2257}$$ 记得在算$kT$的时候转化成电子伏特。
2. 还是列出本征共射电流增益$\beta_0$的公式：$$\beta_0\approx \frac{N_E D_B L_E}{N_B D_E W_{bn}}exp\left(\frac{E_{gE}-E_{gB}}{kT}\right)$$ 所以可以列出一个等式：$$\frac{N_E D_B L_E}{N_B(HBT)D_EW_{bn}}exp\left(\frac{\Delta E_g(HBT)}{kT}\right)=\frac{N_E D_B L_E}{N_B(BJT)D_EW_{bn}}exp\left(\frac{\Delta E_g(BJT)}{kT}\right)$$ 约掉没有关系的东西：$$\frac{1}{N_B(HBT)}exp(\frac{\Delta E_g(HBT)}{kT})=\frac{1}{N_B(BJT)}$$ $$\displaylines{\implies N_B(HBT)=N_B(BJT)\cdot exp(\Delta E_g(HBT)/kT)\\=10^{15}\times e^{0.2/0.0259}=2.257\times 10^{18}cm^{-3}}$$

## Technologies Available

### $\mathrm{GaAs/AlGaAs}$ HBTs

The bandgap of $\mathrm{AlGaAs}$ can be made much higher than $\mathrm{GaAs}$ and be used as an emitter material for HBT. 
$$E_g(x)=1.42+1.247x\ \left(eV\right),\ x<0.45$$
$\mathrm{Al_x Ga_{1-x}}$ is [[Lattice-Matched Heterostructures|Lattice Match]] to $\mathrm{GaAs}$ for all composition $x$. $\mathrm{GaAs}$, with a high bandgap ($1.42eV$) compared to $\mathrm{Si}$, can form a high-quality substrate.

![[npn HBT structure.png|(a) Schematic cross section of an n-p-n HBT structure, (b) Energy band diagram of a HBT operated under active mode.]]
The common emitter current gain varies with the mole fraction of $\mathrm{Al}$.

### $\mathrm{InGaAs/InP}$ and $\mathrm{InGaAs/InAlAs}$ HBTs

- The $\mathrm{InP}$ based $\mathrm{In_{0.53}Ga_{0.47}As}$ ($E_g\cong 0.75eV$) and $\mathrm{In_{0.52}Al_{0.48}As}$ ($E_g=1.4eV$) are lattice matched to $\mathrm{InP}$ ($E_g=1.35eV$)
- $\mathrm{InGaAs}$ has smallest $E_g$ and should be used as base
- The $\mathrm{InGaAs/InP}$ (emitter) structure has very low [[Surface Recombination]]. And electrons have higher [[Carrier Mobility]] in $\mathrm{InGaAs}$ than in $\mathrm{GaAs}$. Such HBTs have a cutoff frequency of **254GHz**.
- Collector can be any one as long as the requirement for breakdown voltage can be met.

![[Pasted image 20241101045310.png#pic_center|InAlAs as the emitter]]

![[Pasted image 20241101045330.png#pic_center|InP as the emitter]]

![[Pasted image 20241101045444.png#pic_center|Current gain as a function of operating frequency for an InGaAs/InP HBT.]]

### $\mathrm{Si/Si_x Ge_{1-x}}$ HBTs

- The alloy $\mathrm{Si_x Ge_{1-x}}$ will be the base due to a smaller band gap.
- $\mathrm{Si/SiGe}$ system is attractive for HBT due to:
	- high speed capability
	- small trap density at $\mathrm{Si}$ surface which minimizes [[Surface Recombination]] current and ensures a high current gain even at low collector current
	- compatibility with standard $\mathrm{Si}$ technology
![[Pasted image 20241101043006.png#pic_center|Device structure of an npn Si/SiGe/Si HBT]]
![[Collector and base current versus Vbe for a HBT and BJT.png#pic_center|Collector and base current versus Vbe for a HBT and BJT]]
The $\mathrm{Si/SiGe}$ HBT has a higher current gain than homojunction $\mathrm{Si}$ BJT, but a lower cutoff frequency than $\mathrm{GaAs}$ and $\mathrm{InP}$-based HBTs because of the lower carrier mobility in $\mathrm{Si}$.

## The Ways to Further Improve HBTs’ Performance

### Emitter Region

The conduction band discontinuity $\Delta E_C$ between the emitter and base is not desirable, since it will make the electrons to transport by means of [[Thermionic Emission]] across a barrier or by tunneling through it.

![[Pasted image 20241101045956.png#pic_center|]]

Therefore, the emitter efficiency and the collector current will suffer.

The problem can be alleviated by using improved structures such as using an emitter with a graded-layer near the E-B junction.

The figure shows an energy band diagram in which the $\Delta E_C$ is eliminated by a graded layer placed between the emitter and base heterojunction. The thickness of the graded layer is $W_g$.

![[Pasted image 20241101050118.png#pic_center|The dashed line shows the energy bandgap of the graded layer.]]


### Base Region

- The base region can also have a graded profile, which results in a reduction of the bandgap from the emitter side to the collector side.
- There is an electric field $\xi_{bi}$ ($\xi=\frac{1}{q}\frac{\mathrm{d}E}{\mathrm{d}x}$) in the quasi-neutral base. It results in a reduction in the minority carrier transit time and, thus, an increase in the common-emitter current gain and the cutoff frequency of the HBT.
- $\xi$ can be realized by varying linearly the $\mathrm{Al}$ [[Vegard’s Law#^648b21|Mole Fraction]] $x$ of $\mathrm{Al_x Ga_{1-x} As}$ in the base from $x=0.1$ to $x=0$.

### Collector Region

- Two factors need to be considered for the collector layer:
	- the transit time delay
	- the breakdown voltage
- A thicker collector layer will improve the breakdown voltage of the B-C junction but increase the transit time.
- In most devices for high-power applications, the carriers move through the collector at their saturation velocities but they need very large-electric fields to be maintained in this layer.
- It is possible to increase the velocities by lowering the electric field with certain doping profile in the collector layer. #TODO 
	- One way is to use $p^−$ or $i$ collectors with a $p^+$ pulse-doped layer near the subcollector for an n-p-n HBT.![[Pasted image 20241101051828.png#pic_center|]]Electrons entering the collector layer can maintain their higher mobility during most of the collector transit time due to the **slightly doped** $p^-$ collector (less impurity scattering). Such a device is called a **ballistic collector transistor (BCT)**.

## SUMMARY

（这AI写的吧）
- The current gain and frequency limitations of a conventional bipolar junction transistor are the result of the [[Heterojunction Electronic Devices#^099bec|Bandgap Shrinkage]] of emitter at high doping, low base doping and relatively wide base. To overcome these limitations, a heterojunction bipolar transistor (HBT) formed by using a wider bandgap semiconductor as emitter can have much high base doping and a much narrower base. The HBT has gained popularity in millimeter-wave and high-speed digital applications.
- The [[Heterojunction Electronic Devices#Technologies Available|Technologies Available]] include $\mathrm{GaAs/AlGaAs}$ lattice matched to $\mathrm{GaAs}$ substrate, $\mathrm{InGaAs/InAlAs}$ lattice matched to $\mathrm{InP}$ substrate and $\mathrm{Si/SiGe}$ on $\mathrm{Si}$ substrate. Among them, the $\mathrm{InP}$ based HBTs ($\mathrm{InP/InGaAs/InP}$ or $\mathrm{InAlAs/InGaAs/InP}$) can have a cutoff frequency of **250GHz**.
- The **[[Heterojunction Electronic Devices#Emitter Region|Bandgap Discontinuity]]** $\Delta E_C$ between the emitter and base is **not desirable** since the carriers need to overcome a barrier, which makes the emitting efficiency and collector current suffer. The problems can be alleviated by improved structures such as the **graded-layer**.
- [[Heterojunction Electronic Devices#Base Region|Graded-base]] and $i$ collector with a $p^+$ pulse-doped layer near the subcollector can also improve device performance.

# Modulation-doped Field Effect Transistors (MODFETs)

![[Pasted image 20241101052703.png#pic_center|]]
- In a FET there is a gate-controlled channel through which current is allowed to flow.
- The gate must be isolated from the channel current flow. Otherwise, an input signal current, while on its way to the output, would “leak” through the gate, leading to a poor gain for the FET.

### Two types of conventional FETs

![[Pasted image 20241101052714.png#pic_center|]]
1. Metal Oxide Semiconductor FETs (MOSFETs)
	- The gate isolation is provided by depositing an oxide between the gate and the active channel.
	- **The n-channel is induced at the p-type $\mathrm{Si}$ surface due to strong inversion associated with band bending and controlled by gate voltage $V_{GS}$.**
	- The electron flow in the channel forms current $I_{DS}$ when $V_{GS}> V_T$ , and $V_{DS}>0$.
2. Metal Semiconductor FETs (MESFETs)
	- In a Metal Semiconductor FET (**no oxide**), the metal gate forms a Schottky barrier with the semiconductor.
	- **The n-channel is a part of the n-type Si, which is not covered by the depletion region of the Schottky barrier, and controlled by the reverse-biased Shottky contact.**

### New FETs Developed Using Heterostructures

- Modulation-doped Field Effect Transistors (MODFETs)
- They are also called:
	- Heterostructure Insulated Gate FETs (HIGFETs)
	- High Electron Mobility Transistors (HEMTs)
	- Two-dimensional Electron Gas FETs (TEGFETs)

## Device Structures