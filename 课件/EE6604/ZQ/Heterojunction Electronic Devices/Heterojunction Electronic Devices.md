---
aliases:
  - Modulation-doped Field Effect Transistors
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

[[HBT]]

# Modulation-doped Field Effect Transistors (MODFETs)

[[MODFET]]
