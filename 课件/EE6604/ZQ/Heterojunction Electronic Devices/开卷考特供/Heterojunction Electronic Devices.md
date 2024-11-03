# Fundamentals

- A heterojunction is defined as a junction (structure) formed by two different semiconductor materials.
- Such semiconductors are mostly alloy (compound) semiconductors
- Examples:
	- $\mathrm{Si Ge_{1-x}}$ on $\mathrm{Si}$
	- $\mathrm{Al_x Ga_{1-x} As}$ on $\mathrm{GaAs}$
	- $\mathrm{Ga_x In_{1-x} As}$ on $\mathrm{Al_x Ga_{1-x} As}$
	- etc.

## Material Parameters of Alloy Semiconductors

- An **alloy semiconductor is a combination of two or more semiconductors**, elemental semiconductors ($\mathrm{Si}$ with $\mathrm{Ge}$) or semiconductor compound from the same group ($\mathrm{GaAs}$ with $\mathrm{InAs}$ or $\mathrm{ZnS}$ with $\mathrm{ZnSe}$).
- An alloy is formed from a physical mixture of two or more compounds, while a compound is formed from a chemical reaction. $\mathrm{GaAs}$ (or $\mathrm{InAs}$) is a compound semiconductor.
- $\mathrm{Ga_{1−x} In_x As}$ is an alloy compound consisting of $\mathrm{GaAs}$ and $\mathrm{InAs}$ with a mole ratio of $(1−x):x$.
- **Alloy semiconductors** could be binary ($\mathrm{SiGe}$, $\mathrm{GaAs}$, $\mathrm{InP}$), or ternary ($\mathrm{Al_x Ga_{1-x} As}$, $\mathrm{In_x Al_{1-x} As}$), or quaternary ($\mathrm{In_x Ga_{1-x} As_y P_{1-y}}$).
- The material parameters include energy bandgap, lattice constant, thermal conductivity, melting point, etc. The first two, **Energy Bandgap** and **Lattice Constant** are the most important ones.

#### Vegard's Law

- Usually, the parameters of the binary materials are known. The parameters of the ternaries and quaternaries can be derived using Vegard’s Law. (In 1921 by Lars Vegard, a Norwegian physicist)
- For a **ternary compound $A_xB_{1-x}C$** (where $A$ and $B$ are the same group elements (group III or group V elements), the parameter $P$, which may be **bandgap** $E_g$ or **lattice constant** (*LC*), can be expressed as $$P\left(A_xB_{1-x}C\right)=xP_{AC}+\left(1-x\right)P_{BC}$$

##### Ternary Compound

- For a **ternary compound** $A_xB_{1-x}C$ (where $A$ and $B$ are the same group elements (group III or group V elements), the parameter $P$, which may be **bandgap** $E_g$ or Lattice Constant ($LC$), can be expressed as $$P(A_xB_{1-x}C)=xP_{AC}+(1-x)P_{BC}$$ where $x$ is **mole fraction** or composition which can vary from 0 to 1. ^648b21

##### Quaternary Compound

- For a **quaternary compound** $A_xB_{1-x}C_yD_{1-y}$ (where $A$ and $B$ are the same group of elements, and $C$ and $D$ are the same group of elements), the parameter $P$ can beobtained from the respective values of the four binaries. $$P\left(A_xB_{1-x}C_yD_{1-y}\right)=xyP_{AC}+x(1-y)P_{AD}+(1-x)yP_{BC}+(1-x)(1-y)P_{BD}$$

##### Ternary Alloys

- If the parameters of the ternary alloys $A_xB_{1-x}C$, $A_xB_{1-x}D$, $AC_yD_{1-y}$, and $BC_yD_{1-y}$ are available, then parameter P can be modified as $$P(A_xB_{1-x}C_yD_{1-y})=\frac{x(1-x)[(1-y)P_{ABD}+yP_{ABC}]}{x(1-x)+y(1-y)}+\frac{y(1-y)[xP_{ACD}+(1-x)P_{BCD}]}{x(1-x)+y(1-y)}$$

### Lattice Constant

- Lattice constant follows Vegard’s Law well.
- Example:
	- $\mathrm{LC (InAs): 6.0583} \mathrm{\overset{\circ}{A}}$
	- $\mathrm{LC (GaAs): 5.6533} \mathrm{\overset{\circ}{A}}$
	- $\mathrm{LC (In_{0.3} Ga_{0.7} As): 0.3 \times 6.0583 + 0.7\times 5.6533 = 5.7748 \overset{\circ}{A}}$, or $\mathrm{0.57748nm}$

![[Lattice Constant.png#pic_center|]]
晶格常数一般由6个参数组成：$a$、$b$、$c$、$\alpha$、$\beta$、$\gamma$
由于在半导体中一般为立方结构，所以可以只用一个参数表示晶胞的物理尺寸。

#### Lattice Constant Variation as a Function of Mole Fraction

![[Lattice Constant Variation as a Function of Mole Fraction.png#pic_center]]

### Energy Bandgap

- The bandgaps of the Ternary Compound and Quaternary Compound semiconductors only approximately follow Vegard’s Law. $$E_g(A_xB_{1-x}C)=xE_g(AC)+(1-x)E_g(BC)$$
- In most alloys, there is a **bowing effect** arising from the increasing disorder due to alloying of different elements. The energy bandgap of alloy semiconductors can bebetter described by the following expression: $$E_g(\mathrm{alloy})=a+bx+cx^2$$

![[Compositional Dependence of Energy Bandgap.png#pic_center|Compositional Dependence of Energy Bandgap of the III-V Alloys at 300 K]]

## Lattice Match and Mismatch Heterostructures

- There are two kinds of heterostructures:
	- **Lattice-Matched Heterostructures**
		- The two materials have the same Lattice Constants, e.g. AlAs on GaAs.
		  两种材料有相同的晶格常数。
	- **Lattice-Mismatched Heterostructures**
		- The **lattice-mismatched heterostructures** can be further classified as **Strained Heterostructure** and **Unstrained Heterostructure**.

![[Lattice Match and Mismatch Heterostructures.png#pic_center|Lattice Match and Mismatch Heterostructures]]

### Strained Heterostructure


![[Pasted image 20241030011450.png#pic_center|Strained Heterostructure]]

- Assume
	- $a_s$ Lattice Constant of Si substrate
	- $a_f$ Lattice Constant of the SiGe bulk film
- If the epitaxially grown SiGe is **very thin**, the heterostructure will be **strained**.
- In this case, the normal cubic unit cell of the grown SiGe film $a_f\cdot a_f\cdot a_f$, will be distorted to a tetragonal cell $a_{f\parallel}\cdot a_{f\parallel}\cdot a_{f\perp}$. That is, $a_{f\parallel}=a_s$, $a_{f\perp}\neq a_{f\parallel}$ and $a_f\neq a_{f\perp}$.

- The strain parallel to the interface is $$\epsilon_\parallel=\frac{a_{f\parallel}-a_f}{a_f}=\frac{a_s-a_f}{a_f}$$
- The strain perpendicular to the interface $$\epsilon_\perp=\frac{a_{f\perp}-a_f}{a_f}$$
- The substrate-film lattice mismatch (or misfit) is defined as: $$M=\frac{a_s-a_f}{a_f}$$$M$ is the same as the parallel strain. ^5aff88

### Unstrained Heterostructure

- If the growing $SiGe$ film is **thick** enough, the heterostructure will be **unstrained**.
- In this case, the grown film and the substrate have their own bulk lattice constants.
- The two materials, $SiGe$ film and Si substrate have cubic symmetry. That is, the cubic unit cell $a_f\cdot a_f\cdot a_f$ is for the film and $a_s\cdot a_s\cdot a_s$ is for the substrate.

![[Pasted image 20241030012030.png#pic_center|Unstrained Heterostructure]]

- In this case, the atoms of the film and the substrate do **NOT** have a one-to-one correspondence at the interface. 
- This results in the formation of defects at the interface of the two materials, called **misfit dislocations**.

### Critical Thickness

- There is a critical thickness $h_c$ below which the film grown is strained without misfit dislocation (**pseudomorphic growth**), and above which the film becomes unstrained or relaxed, associated with formation of misfit dislocations at the interface. $$h_c=\frac{b}{8\pi(1+v)M}\left[ln\left(\frac{h_c}{b}\right)+1\right]$$
- where $b=\frac{b}{\sqrt{2}}$ for most (100) semiconductor systems (a is Lattice Constant]of substrate), $v$ is Poisson's ratio with an approximate value of 0.274, $M$ is the **Mismatch**.

> ### Mismatch
> $$M=\frac{a_s-a_f}{a_f}$$
> ### Poisson's ratio 泊松系数
> 泊松系数指的是在固体力学中，材料的横向变形系数，即泊松比，称为泊松系数。


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

- Consider the energy band diagrams for two materials with different Electron Affinity $\mathrm{q}\chi$ , the energy gaps $E_g=E_c-E_v$ and the chemical potentials or Fermi Level|Fermi Energy $E_f$.
- Note:
	- Vacuum Level must be continuous
	- The band bending upward means an increase in electron energy, decrease in electron density
	- The band bending downward means a decrease in electron energy, increase in electron density

> ### Electron Affinity 电子亲和能
> 电子亲和能是导带最小值与真空能级之间的能量差。它表示电子从真空能级进入导带的难易程度，通常在讨论半导体的掺杂和表面态时非常关键。符号为$\chi$

>  ### Vacuum Level 真空能级
>  代表电子在材料外部静止时的能量，是所有其他能量的参考点。

> ### Fermi Level 费米能级
> 在费米-狄拉克分布中，费米能级可视为热力学平衡时，电子有50%概率占据的假想能级。
> 
> - 绝缘体中，$E_F$位于能隙上，与导带和价带相距甚远。
> - 金属、半金属中，$E_F$位于导带上。
> - 无杂质半导体或少量掺杂的半导体中，$E_F$虽位于能隙上，但与导带和价带较近。
> 
> - 在掺杂的半导体中，费米能级会产生偏移。
	- 对于N型半导体，费米能级为：$$E_F-E_i=kTln\left(\frac{N_d}{n_i}\right)$$
	- P型半导体的费米能级为：$$E_i-E_F=kTln\left(\frac{N_a}{n_i}\right)$$ $N_d$为施主浓度；$N_a$为受主浓度；$E_i$为本征费米能级

### Bandgap Offset

![[Bandgap Offset.png|Bandgap Offset]]

$$\displaylines{
\Delta E =& E_{g1}-E_{g2}=\Delta E_C+\Delta E_V \\
\Delta E_C =& E_{C1}-E_{C2} \\
\Delta E_V =& E_{V2}-E_{V1}
}$$
- The ratio $\Delta E_C/\Delta E_V$ varies with material systems and is not easy to be determined.
- The $\mathrm{GaAs/AlAs}$ and $\mathrm{GaAs/AlGaAs}$ systems have type I structure, and the ratio $\Delta E_C/\Delta E_V$ is about 60:40.

- The band diagram of Metal/AlGaAs/GaAs Heterostructure under Thermal Equilibrium
![[Pasted image 20241030020138.png#pic_center|The band diagram of Metal/AlGaAs/GaAs Heterostructure]]

> ### Thermal Equilibrium 热平衡
> 在半导体中指材料中的载流子，产生数等于复合数。

# Heterojunction Bipolar Transistors (HBTs)

The bandgap of a Ternary or Auaternary Alloy semiconductor can be varied, by simply adjusting the composition $x$ or $y$.
三元合金或四元合金半导体的带隙可以通过简单地调整组成$x$或$y$来改变。

The heterostructures formed by alloy semiconductors, therefore, have immense applications in various fields.
因此，合金半导体形成的异质结在各个领域都有巨大的应用。

## Limitations of Homojunction BJTs

![[HBT_FIG1.png|Carrier Distribution]]

- The Emitter Injection Efficiency $\gamma$ is: $$\gamma=\frac{I_{En}}{I_{En}+I_{Ep}}$$ since $I_{Ep} \ll E_{En}$, if follows: $$\gamma=1-\frac{p_{E0}D_E W_{bn}}{n_{B0}D_BL_E}$$ where,
	- $p_{E0}$: Equilibrium hole concentration in the emitter
	- $n_{B0}$: Equilibrium electron concentration in the base
	- $W_{bn}$: Neutral width of the base
	- $D_E$, $D_B$: Diffusion coefficients of minority carriers in emitter and base respectively
	- $L_E$: Diffusion length of minority carriers in the emitter
- The Base Transport Factor $\alpha_T$ is: $$\alpha_T=\frac{I_{Cn}}{I_{En}}\approx \frac{I_C}{I_{En}}=1-\frac{W_{bn}^2}{2L_B^2}$$ where, 
	- $L_B$: The diffusion length of minority carriers in the base
- The Common Base Current Gain $\alpha_0$ is: $$\alpha_0=\frac{I_C}{I_E}=\frac{I_C}{I_{En}}\cdot \frac{I_{En}}{I_E}=\alpha_T\cdot \gamma$$ Substituting the expressions for $\alpha_T$ and $\gamma$, we get $$\alpha_0=\left[1-\frac{W_{bn}^2}{2L_B^2}\right]\cdot \left[1-\frac{p_{E0}D_E W_{bn}}{n_{B0}D_B L_E}\right]$$
- The Common Emitter Current Gain $\beta_0$ is: $$\beta_0=\frac{\alpha_0}{1-\alpha_0}\approx\frac{n_{B0}D_B L_E}{p_{E0}D_EW_{bn}}$$ To achieve a high $\beta_0$, 
	- $p_{E0} \ll n_{B0} \implies n_{E0} \gg p_{B0}$
	- $W_{bn}$ is very small, and $W_{bn} \ll L_B$
  These mean
	- Emitter doping should be very high and base doping should be relatively much lower.
	- The base should be very narrow.

> ### Common Base Current Gain 共基极电流增益
> $$\alpha=\frac{I_C}{I_E}=\frac{\beta}{\beta+1}$$
> ### Common Emitter Current Gain 共发射极电流增益
> $$\beta=\frac{I_C}{I_B}=\frac{\alpha}{1-\alpha}$$

### Limitations

- Too narrow and lightly doped base will result in
  基区过窄和轻掺杂会导致：
	- Large base resistance
	  基区电阻大
	- Smaller breakdown voltage
	  击穿电压小
- Too heavy doping in emitter will cause bandgap of emitter to shrink.
  发射极重掺杂会导致带隙缩小

It will then cause the base injection to increase, emitter injection to decrease and eventually leading to decrease in the emitter efficiency and current gain.
这将导致基极注入增加，发射极注入减少，最终导致发射极效率和电流增益降低。

#### Effect of Emitter Doping

The bandgap shrinkage caused by heavy doping in the n-type emitter results in a higher barrier for electron injection and lower barrier for hole injection. ^099bec
n型发射极中重掺杂引起的带隙缩小导致电子注入的势垒更高，空穴注入的势垒更低。

![[HBT_FIG2.png]]

In Si, the bandgap shrinkage due to doping is approximately given by $$\Delta E_g=-22.5\left(\frac{N_d}{10^{18}}\cdot\frac{300}{T}\right)^{1/2}(meV)$$
and the Common Emitter Current Gain becomes $$\beta\approx \beta_0 exp(-\frac{\left|\Delta E_g\right|}{kT})$$ decreasing with heavy doping.

Thereffore, with a simple n-p homojunction for the emitter-base, the performance of the npn BJT is limited.
因此，由于BE区采用简单的n-p同质结，npn BJT的性能受限。

## Remedy

- Use a large bandgap material for n-type emitter. The deivce will then become a heterojunction bipolar transistor (HBT)
- The main advantage of HBT is the high emitter efficiency
- HBTs also have high speed and high frequency capability in circuit operation

![[HBT_FIG3.png|A HBT with an n-AlGaAs emitter and a p-GaAs base transistor (a) Device structure, (b) Band diagram at thermal equilibrium]]

### Common Emitter Current Gain of HBTs

- From the definition, $$\beta_0\approx\frac{n_{B0}D_B L_E}{p_{E0}D_E W_{bn}}$$ and from **Law of Mass Action**, $np=n_i^2$, the minority carrier concentration in the emitter $p_{E0}$, is $$p_{E0}=\frac{n_o^2(\text{emitter})}{N_E(\text{emitter})}=\frac{N_CN_V exp(-\frac{E_{gE}}{kT})}{N_E}$$ where,
	- $N_C$: Effective Density of States in the conduction band
	- $N_V$: Effective Density of States in the valence band
	- $E_{gE}$ is the bandgap of the emitter
- The minority carrier concentration in the base $n_{B0}$ is $$n_{B0}=\frac{n_i^2(\text{base})}{N_B(\text{base})}=\frac{N_C^\prime N_V^\prime exp(-\frac{E_{gB}}{kT})}{N_B}$$ where, 
	- $N_C^\prime$ and $N_V^\prime$: Effective Density of States in conduction band and valence band respectively
	- $E_{gB}$: bandgap of base

> ### Law of Mass Action
> $$p_0n_0=n_i^2$$
> $E_g$为半导体的禁带宽度。
> $p_0$和$n_0$为两种**平衡载流子浓度**
> 由于电中性，在本征半导体中有$p_i=n_i$

> ### Equilibrium Carrier Concentration 平衡载流子浓度
> 在硅和其他半导体中，导带热平衡载流子浓度：$$n_0=N_c\times exp\left(-\frac{E_c-E_F}{kT}\right)$$
> 价带热平衡载流子浓度：$$p_0=N_v\times exp\left(-\frac{E_F-E_v}{kT}\right)$$
> - 符号：
> 	- $n_0$: [[Thermal Equilibrium|热平衡]]电子浓度
> 	- $p_0$: [[Thermal Equilibrium|热平衡]]空穴浓度
> 	- $N_c$: 导带[[Effective Density of States|有效态密度]]
> 	- $N_v$: 价带[[Effective Density of States|有效态密度]]
> 	- $E_F$: [[Fermi Level|费米能级]]
> 	- $k$: 玻尔兹曼常数
> 	- $T$: 开尔文温度

Hence $$\displaylines{\beta_0=\frac{n_{B0}D_B L_E}{p_{E0} D_E W_{bn}}\approx \frac{N_E D_B L_E}{N_B D_E W_{bn}}exp(\frac{E_{gE}-E_{gB}}{kT})\\=\frac{N_E D_B L_E}{N_B D_E W_{bn}}exp(\frac{\Delta E_g}{kT})}$$

![[HBT_FIG4.png#pic_center]]
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
2. 还是列出本征共射电流增益$\beta_0$的公式：$$\beta_0\approx \frac{N_E D_B L_E}{N_B D_E W_{bn}}exp\left(\frac{E_{gE}-E_{gB}}{kT}\right)$$ 所以可以列出一个等式：$$\displaylines{\frac{N_E D_B L_E}{N_B(HBT)D_EW_{bn}}exp\left(\frac{\Delta E_g(HBT)}{kT}\right)\\=\frac{N_E D_B L_E}{N_B(BJT)D_EW_{bn}}exp\left(\frac{\Delta E_g(BJT)}{kT}\right)}$$ 约掉没有关系的东西：$$\frac{1}{N_B(HBT)}exp(\frac{\Delta E_g(HBT)}{kT})=\frac{1}{N_B(BJT)}$$ $$\displaylines{\implies N_B(HBT)=N_B(BJT)\cdot exp(\Delta E_g(HBT)/kT)\\=10^{15}\times e^{0.2/0.0259}=2.257\times 10^{18}cm^{-3}}$$

## Technologies Available

### $\mathrm{GaAs/AlGaAs}$ HBTs

The bandgap of $\mathrm{AlGaAs}$ can be made much higher than $\mathrm{GaAs}$ and be used as an emitter material for HBT. 
$$E_g(x)=1.42+1.247x\ \left(eV\right),\ x<0.45$$
$\mathrm{Al_x Ga_{1-x}}$ is Lattice Match to $\mathrm{GaAs}$ for all composition $x$. $\mathrm{GaAs}$, with a high bandgap ($1.42eV$) compared to $\mathrm{Si}$, can form a high-quality substrate.

![[HBT_FIG5.png|(a) Schematic cross section of an n-p-n HBT structure, (b) Energy band diagram of a HBT operated under active mode.]]
The common emitter current gain varies with the mole fraction of $\mathrm{Al}$.

### $\mathrm{InGaAs/InP}$ and $\mathrm{InGaAs/InAlAs}$ HBTs

- The $\mathrm{InP}$ based $\mathrm{In_{0.53}Ga_{0.47}As}$ ($E_g\cong 0.75eV$) and $\mathrm{In_{0.52}Al_{0.48}As}$ ($E_g=1.4eV$) are lattice matched to $\mathrm{InP}$ ($E_g=1.35eV$)
- $\mathrm{InGaAs}$ has smallest $E_g$ and should be used as base
- The $\mathrm{InGaAs/InP}$ (emitter) structure has very low **Surface Recombination**. And electrons have higher Carrier Mobility in $\mathrm{InGaAs}$ than in $\mathrm{GaAs}$. Such HBTs have a cutoff frequency of **254GHz**.
- Collector can be any one as long as the requirement for breakdown voltage can be met.

![[HBT_FIG6.png#pic_center|InAlAs as the emitter]]

![[HBT_FIG13.png#pic_center|InP as the emitter]]

![[HBT_FIG7.png#pic_center|Current gain as a function of operating frequency for an InGaAs/InP HBT.]]

### $\mathrm{Si/Si_x Ge_{1-x}}$ HBTs

- The alloy $\mathrm{Si_x Ge_{1-x}}$ will be the base due to a smaller band gap.
- $\mathrm{Si/SiGe}$ system is attractive for HBT due to:
	- high speed capability
	- small trap density at $\mathrm{Si}$ surface which minimizes Surface Recombination current and ensures a high current gain even at low collector current
	- compatibility with standard $\mathrm{Si}$ technology

> ### Surface Recombination 表面复合
> 半导体的表面充满缺陷（悬空的键和环境中的杂质），这导致表面态和表面附近的能带弯曲。所以在未钝化的半导体表面，非辐射复合的速度更快。
> 关于表面复合的速度：$$\text{recombination\ rate}=S_eA\left(n-n_0\right)$$
> 上式中：
> - $S_e$表示表面复合速度$cm/s$
> - $A$表面的面积$cm^2$
> 所以符合速度的单位是$s^{-1}$

![[HBT_FIG8.png#pic_center|Device structure of an npn Si/SiGe/Si HBT]]
![[HBT_FIG9.png#pic_center|Collector and base current versus Vbe for a HBT and BJT]]
The $\mathrm{Si/SiGe}$ HBT has a higher current gain than homojunction $\mathrm{Si}$ BJT, but a lower cutoff frequency than $\mathrm{GaAs}$ and $\mathrm{InP}$-based HBTs because of the lower carrier mobility in $\mathrm{Si}$.

## The Ways to Further Improve HBTs’ Performance

### Emitter Region

The conduction band discontinuity $\Delta E_C$ between the emitter and base is not desirable, since it will make the electrons to transport by means of **Thermionic Emission** across a barrier or by tunneling through it.

> ### Thermionic Emission
> 一种通过热激发发射载流子的方式。
> 
> 这个现象发生的原因是，提供给载流子的热能使它们能够克服束缚势能（在金属材料中，这束缚势能也被称为逸出功。通过热发射产生的载流子可能是电子或者离子。发射载流子之后原始区域会产生一个于被发射载流子总和大小相同、极性相反的载流子。产生电子的热发射被称为**热电子发射**。
> > ### Work Function 逸出功
> > 指要使一粒电子立即从固体内部移到固体外部，所必须提供的最小能量。半导体为费米能级到真空能级的能量。**注意与电子亲和能区分**

![[HBT_FIG10.png#pic_center]]

Therefore, the emitter efficiency and the collector current will suffer.

The problem can be alleviated by using improved structures such as using an emitter with a graded-layer near the E-B junction.

The figure shows an energy band diagram in which the $\Delta E_C$ is eliminated by a graded layer placed between the emitter and base heterojunction. The thickness of the graded layer is $W_g$.

![[HBT_FIG11.png#pic_center|The dashed line shows the energy bandgap of the graded layer.]]


### Base Region

- The base region can also have a graded profile, which results in a reduction of the bandgap from the emitter side to the collector side.
- There is an electric field $\xi_{bi}$ ($\xi=\frac{1}{q}\frac{\mathrm{d}E}{\mathrm{d}x}$) in the quasi-neutral base. It results in a reduction in the minority carrier transit time and, thus, an increase in the common-emitter current gain and the cutoff frequency of the HBT.
- $\xi$ can be realized by varying linearly the $\mathrm{Al}$ Mole Fraction $x$ of $\mathrm{Al_x Ga_{1-x} As}$ in the base from $x=0.1$ to $x=0$.

### Collector Region

- Two factors need to be considered for the collector layer:
	- the transit time delay
	- the breakdown voltage
- A thicker collector layer will improve the breakdown voltage of the B-C junction but increase the transit time.
- In most devices for high-power applications, the carriers move through the collector at their saturation velocities but they need very large-electric fields to be maintained in this layer.
- It is possible to increase the velocities by lowering the electric field with certain doping profile in the collector layer.
	- One way is to use $p^−$ or $i$ collectors with a $p^+$ pulse-doped layer near the subcollector for an n-p-n HBT.
![[HBT_FIG12.png#pic_center]]Electrons entering the collector layer can maintain their higher mobility during most of the collector transit time due to the **slightly doped** $p^-$ collector (less impurity scattering). Such a device is called a **ballistic collector transistor (BCT)**.

## SUMMARY

（这AI写的吧）
- The current gain and frequency limitations of a conventional bipolar junction transistor are the result of the **Bandgap Shrinkage** of emitter at high doping, low base doping and relatively wide base. To overcome these limitations, a heterojunction bipolar transistor (HBT) formed by using a wider bandgap semiconductor as emitter can have much high base doping and a much narrower base. The HBT has gained popularity in millimeter-wave and high-speed digital applications.
- The Technologies Available include $\mathrm{GaAs/AlGaAs}$ lattice matched to $\mathrm{GaAs}$ substrate, $\mathrm{InGaAs/InAlAs}$ lattice matched to $\mathrm{InP}$ substrate and $\mathrm{Si/SiGe}$ on $\mathrm{Si}$ substrate. Among them, the $\mathrm{InP}$ based HBTs ($\mathrm{InP/InGaAs/InP}$ or $\mathrm{InAlAs/InGaAs/InP}$) can have a cutoff frequency of **250GHz**.
- The **Bandgap Discontinuity** $\Delta E_C$ between the emitter and base is **not desirable** since the carriers need to overcome a barrier, which makes the emitting efficiency and collector current suffer. The problems can be alleviated by improved structures such as the **graded-layer**.
- Graded-base and $i$ collector with a $p^+$ pulse-doped layer near the subcollector can also improve device performance.

# Modulation-doped Field Effect Transistors (MODFETs)


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
	- In a Metal Semiconductor FET (**no oxide**), the metal gate forms a Schottky Barrier with the semiconductor.
	- **The n-channel is a part of the n-type Si, which is not covered by the depletion region of the Schottky Barrier, and controlled by the reverse-biased Shottky contact.**

> ### Schottky-Barrier 肖特基势垒
> #### 热平衡
> 在金属与半导体接触中，形成肖特基势垒的接触称为肖特基接触或者整流接触。一般都是金属与一个n型半导体接触。
> 
> 符号：
> - 金属的功函数$e\phi_m$
> - n型半导体的功函数$e\phi_s$
> - n型半导体的电子亲和能$\chi$
> ![[Pasted image 20241102020725.png]]
> 在n型半导体与金属发生接触时，由于真空能级必须连续，所以n型半导体的导带发生弯曲以匹配金属的功函数。同时二者作为一个热平衡的系统，费米能级必须相同，所以在远处n型半导体与金属的费米能级必须在同一能级上。
> 
> 所以就发生如图的能带弯曲，规定：
> - 势垒高度$\phi_{bn}=\phi_m-\chi /e$为金属中电子试图进入半导体时所遇到的势垒，这一势垒就是**肖特基势垒**
> - 内建势垒$V_D=\phi_{bn}-\phi_n$，其中$e\phi_n$为n型半导体中导带底与费米能级的能量差

## New FETs Developed Using Heterostructures

- Modulation-doped Field Effect Transistors (MODFETs)
- They are also called:
	- Heterostructure Insulated Gate FETs (HIGFETs)
	- High Electron Mobility Transistors (HEMTs)
	- Two-dimensional Electron Gas FETs (TEGFETs)

## Device Structures

![[MODFET_FIG3.png|A systematic of a GaAs/AlGaAs n-MODFET]]
1. Semi-Insulating GaAs Substrate.
   半绝缘GaAs
2. Undoped GaAs, 2-dimensional $e$ gas is formed on the surface of this layer.
   未掺杂的GaAs，这个区域会形成二维电子气
3. Undoped AlGaAs as a spacer which separates the electrons in undoped GaAs and the donor ions in doped AlGaAs.
   未掺杂的AlGaAs形成间隔层，将未掺杂GaAs层的电子和掺杂的AlGaAs层的施主离子隔离
4. Donor-doped AlGaAs.
   施主掺杂的AlGaAs
5. Metal gate which forms Schottky Barrier with the doped AlGaAs.
   金属栅极，与掺杂的AlGaAs形成肖特基势垒

The energy band profile shows band bending leading to a triangular quantum well at the $\mathrm{GaAs/AlGaAs}$ interface. 
![[MODFET_FIG4.png#pic_center|]]

## Modulation Doping

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

### Advantages of the Modulation Doping

- Because the electrons at the surface of the narrow gap GaAs are spatially separated from the positively charged dopant ions by the undoped AlGaAs spacer, these electrons are virtually free to move in the undoped GaAs channel and essentially remain free from impurity ion scattering. **Thus, they have high mobility**.
  由于在窄带隙GaAs表面的电子从空间上与带正电的杂质离子被未掺杂的AlGaAs隔离层隔离，这些电子在未掺杂的GaAs沟道中几乎可以自由移动，并且基本上不受杂质离子散射的影响。**因此，它们具有高迁移率**。
  ![[MODFET_FIG7.png#pic_center|2-dimensional property]]
- As the trapped electrons have 2-dimensional properties (moving in x-y plane), hence they are called two-dimensional electron gas. The sheet electron concentration is very high as they are limited to a very thin surface layer of the GaAs.
  由于被捕获的电子具有二维特性（在x-y平面内移动），因此它们被称为二维电子气。面电子浓度非常高，因为它们被限制在非常薄的GaAs的表面层。

![[MODFET_FIG8.png#pic_center|]]

- The two-dimensional electron gas has the highest mobility at a **given temperature**. 
- This is why such devices are also called **High Electron Mobility Transistors (HEMTs)**.

## Normally-off and normally-on Devices

- To control the drain-source current $I_D$ by means of a gate voltage $V_G$, the thickness of the wide bandgap layer between the gate metal and the 2DEG is critical.
- By varying the thickness of the wide-bandgap layer, the MODFET can be made either a normally off (enhancement mode) or normally on (depletion mode) device.

### Normally-off or Enhancement-mode MODFETs

- When the wide-bandgap layer is thin, the MODFET will be a normally-off device.
![[Pasted image 20241102014640.png]]
- Energy band diagrams of a normally-off MODFET at
	- (a) Thermal Equilibrium
	- (b) The onset of threshold ($V_T>0$)
- $d_1$ and $d_0$ are the thicknesses of the doped and undoped regions of the wide bandgap semiconductor, respectively
- $\Delta E_C$ is the conduction bandgap offset

- For small AlGaAs thickness, the gate Schottky Barrier can completely deplete the electrons in the AlGaAs as well as the 2DEG even at zero gate bias, thus leading to enhancement-mode type or normally off devices.
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

### Normally-on or Depletion-mode MODFETs

- When the wide bandgap layer is thick enough, the MODFETs will be Normally-on or Depletion-mode devices.
- For thicker AlGaAs layers, the depletion region of the Schottky Barrier does not deplete the electron gas at zero gate voltage ($W<d=d_1+d_0$). Such devices are Normally-on or Depletion-mode devices. (A channel exists at $V_G=0$). ![[Pasted image 20241102030333.png#pic_center|]]

- A negative gate voltage is required to deplete the electron gas and pinch the device off. ($V_T<0$) ![[Pasted image 20241102030724.png#pic_center]]

### Example

Consider an AlGaAs/GaAs heterojunction with n-AlGaAs doped to $2\times 10^{18} cm^{-3}$ and a thickness of $40\mathrm{nm}$. Assume the undoped spacer layer is $3\mathrm{nm}$ and the Schottky barrier height is $0.85e\mathrm{V}$ and $\Delta E_C/q=0.23\mathrm{V}$. The dielectric constant of the AlGaAs is 12.3. Calculate the two-dimensional electron gas concentration for such heterojunction at $V_G=0$.

#### Solution

- 首先判断器件类型（常开还是常闭），判断依据是阈值电压$V_T$ $$V_T=\phi_{Bn}-\frac{\Delta E_C}{q}-V_p$$
	- 肖特基势垒$q\phi_{Bn}=0.85e\mathrm{V}\implies \phi_{Bn}=0.85V$
	- $\frac{\Delta E_C}{q}=0.23V$
	- pinch-off voltage: $$V_p=\frac{qN_Dd_1^2}{2\epsilon_s}$$
		- 掺杂浓度$N_D=2\times 10^{18}\mathrm{cm}^{-3}$
		- AlGaAs厚度$d_1=40\mathrm{nm}=40\times10^{-7}\mathrm{cm}$
		- 相对介电常数$\epsilon_s=12.3$，所以介电常数为$\epsilon_s\cdot\epsilon_0$
		$$\implies V_p=2.35\mathrm{V}$$
	所以阈值电压$V_T$：$$V_T=0.85-0.23-2.35=-1.73\mathrm{V}$$
- 二维电子气浓度$n_s$： $$n_s=\frac{\epsilon_s\epsilon_0}{d_1+d_0+\Delta d}\frac{V_G-V_T}{q}=2.30\times 10^{12}cm^{-2}$$

## Current-Voltage Characteristics

- The current voltage characteristics of a MODFET can be obtained in the way similar to the MOSFET. The current at any point along the channel is $$I_D=Wq\mu_n n_s\xi_y=W\mu_nC_g\left[V_G-V_T-V(y)\right]\frac{\mathrm{d}V(y)}{\mathrm{d}y}$$ Where:
	- $W$ is the channel width
	- $\xi_y$ is longitudinal electric field
- Since the current is constant along the channel, integrating the equation from source to drain ($y=0$ to $y=L$) gives $$I_D=\frac{W}{L}\mu_n C_g\left[(V_G-V_T)V_D-\frac{V_D^2}{2}\right]$$
	- When $V_D\ll(V_G-V_T)$, it is in linear region and $$I_D=\frac{W}{L}\mu_nC_g\left[(V_G-V_T)V_D\right]$$
	- At large drain voltage, the charge sheet $n_s(y)$ at the drain is reduced to 0. So $V_{Dsat}=V_G-V_T$ and the saturation current is $$I_{Dsat}=\frac{W\mu_nC_g}{2L}\left(V_G-V_T\right)^2=\frac{W\mu_n\epsilon_s}{2L(d_1+d_0+\Delta d)}(V_G-V_T)^2$$
	- For high-speed operations, the longitudinal field along the channel is sufficiently high to cause carrier drift velocity saturation ($v_{ds}$). The current (maximum) in the velocity-saturation region is $$I_{Dmax}=qn_sv_{ds}W=C_g(V_G-V_T)v_{ds}W$$
## Important Parameters

### Channel Conductance

$$g_d=\frac{\partial I_D}{\partial V_D}\Bigg|_{V_G}$$
The electron draft velocity is $v_d=\mu\xi$
where:
- $\mu$ is Carrier Mobility
- $\xi$ is electric field and $\xi=\frac{V_D}{L}$ , $L$ is channel length

$$\displaylines{I_D=q n_s v_d W=Wq n_s\mu_n\xi_y=\frac{W}{L}V_D q n_s \mu_n\\\implies g_d=\frac{W}{L}q n_s \mu_n}$$

With $n_s=10^{12}\mathrm{cm^{-2}}$ in a channel $1\mu\mathrm{m}$ long and $10\mu\mathrm{m}$ wide, and $\mu_n$ of electrons in the GaAs channel is $7000cm^2\cdot V^{-1}s^{-1}$, then $g_d=1.12\times 10^{-2}\mathrm{S(siemens)}$, which is **10 times higher** than in a Si MOSFET.

### Transconductance

$$g_m=\frac{\partial I_D}{\partial V_G}\Bigg|_{V_D}\implies g_m(\mathrm{sat})=\frac{\partial}{\partial V_G}C_g v_{ds}W(V_G-V_T)=C_g v_{ds}W$$
- 其中$v_{ds}$是速度饱和的速度

### Transit Time

$$t_r=\frac{L}{v_{ds}}$$
For $L=1\mu\mathrm{m}$ and $v_{ds}=2\times 10^7\mathrm{cm\cdot s^{-1}}$, the transit time is $5\mathrm{ps}$.

MODFETs have very small transit time that enables them to be used as high-speed devices.
## Cutoff Frequency

- The speed of a MODFET is measured by the cutoff frequency $$f_T=\frac{g_m}{2\pi(\mathrm{total\ capacitance})}=\frac{W v_{ds} C_g}{2\pi (WL C_g+C_p)}$$ where:
	- $C_p$ is the parasitic capacitance
- To improve $f_T$, we should consider a semiconductor with large $v_{ds}$, a gate structure with an ultra short gate length, and a device configuration with minimum parasitic capacitance.

### Cutoff Frequency Versus Channel or Gate Length for Five Kinds of Field-Effect Transistors

![[Pasted image 20241102041324.png]]
- The best pseudomorphic SiGe MODFETs have a $f_T$ comparable to the GaAs MODFET. SiGe MODFETs are attractive because they can be processed with silicon fabrication facilities.
- The $\mathrm{Al_{0.48}In_{0.52}As-Ga_{0.47}In_{0.53}As}$ MODFET formed on a InP substrate has higher $f_T$, mainly due to the high electron mobility and velocities in the $\mathrm{Ga_{0.47}In_{0.53}As}$. The $f_T$ at a gate length of $50\mathrm{nm}$ can be as high as $600\mathrm{GHz}$.

## Summary

- The MODFET is a device which enhanced high-frequency performance. This device structure is similar to that of a MESFET except there is a heterojunction under the gate. A two-dimensional electron gas, i.e., a conductive channel, is formed at the heterojunction interface, and electrons with high mobility and high average drift velocity can be transported from the source through the channel to the drain.
  MODFET是一种增强高频性能的器件。其结构类似于MESFET，但在栅极下方有异质结。在异质结界面形成了二维电子气，即导电沟道，具有高迁移率和高平均漂移速度的电子可以从源极通过沟道到达漏极。
- The output characteristics of all field-effect transistors (FETs) are similar. They all have a linear region at low-drain biases. As the bias increases, the output current eventually saturates, and at a sufficiently high voltage, avalanche breakdown occurs at the drain. Depending on whether it requires a positive- or negative-threshold voltage, FET can be either normally off (enhancement mode) or normally on (depletion mode).
  所有场效应晶体管（FET）的输出特性都相似。它们在低漏极偏置时都有一个线性区域。随着偏置的增加，输出电流最终会饱和，并且在足够高的电压下，会在漏极处发生雪崩击穿。根据是否需要正阈值电压或负阈值电压，FET可以是常断型（增强模式）或常通型（耗尽模式）。
- The cutoff frequency $f_T$ is a figure of merit for the high-frequency performance of a FET. The conventional GaAs MODFET and the pseudomorphic SiGe MODFET have a $f_T$ about 30% higher than that of the GaAs MESFET. The GaInAs MODFET has the highest $f_T$ and it has a projected $f_T$ of $600\mathrm{GHz}$ at a gate length of $50\mathrm{nm}$.
  截止频率$f_T$是评估 FET 高频性能的指标。传统的 GaAs MODFET 和伪SiGe MODFET 的$f_T$大约比GaAs MESFET高30%.GaInAs MODFET具有最高的$f_T$,在$50\mathrm{nm}$栅极长度下的$f_T$为$600\mathrm{GHz}$。