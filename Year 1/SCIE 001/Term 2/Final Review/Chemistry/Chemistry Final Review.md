# <center>Chemistry Final Review</center>

## Chemical Kinetics

Mole Fractions: unit of amount of a constituent divided by the total amount of all substituents
$$
\chi_{A}=\frac{n_A}{n_A+n_B}, \chi_{B}=\frac{n_B}{n_A+n_B}, \chi_A + \chi_B = 1
$$

$$
\chi_{solution} \approx 1
$$

Concentration: Experimentally measured

- Pressure for a gas: $P_A = \frac{n_A}{V}RT$
- Absorbance of a solution: $\text{Absorbance} = \epsilon l c$

### Reaction Rate

The **rate** or velocity $v$ of reaction is defined as a ***positive*** quantity

- $A + 2B \to C$
- $v = -\dv{[A]}{t} = -\frac{1}{2}\dv{[B]}{t} = \dv{[C]}{t}$, **stoichiometry** is important
- Rates of chemical reactions must be determined **experimentally**

For a general reaction:
$$
v = \frac{1}{n_1}\dv{P_1}{t} = \frac{1}{n_2}\dv{P_2}{t} = ... = -\frac{1}{m_1}\dv{[R_1]}{t} = -\frac{1}{m_2}\dv{[R_2]}{t}
$$

- $P$: products
- $R$: reactants

Reaction rate is **the slope of a tangent** drawn to the graph of **concentration as a function of time** divided by the **relevant stoichiometric coefficient**

- Average rate: $v_{mean} = \frac{c_2 - c_1}{t_2 - t_1}$
- Instantaneous rate: $v = \dv{c}{t}$

Factors affecting reaction rate

- Nature of reactants and products
- Concentrations of reactants and products
- Temperature (often rate doubles for $10^{\circ}C$ rise in temperature)
- Catalyst / Inhibitor

### Rate Law

Fine the rate: $v = f(concentration, temperature)$

Rate laws can be written as a simple power law
$$
v = -\dv{[A]}{t}=k[A]^a[B]^b[C]^c
$$

- $k$: rate constant
- $a, b, c$: order of the reaction
- **Order of reaction** $\ne$ **Stoichiometric coefficient**

### Rate Constant

The rate constant usually depends on temperature and may also depend on concentration

The units of $k$ must be consistent with the rate units which are usually expressed as concentration over time $\to$ depend on the *reaction order*

- $a$th order in $A$, $b$th order in $B$, $c$th order in $C$
- Overall order of reaction: $n=a+b+c+...$
- The units of $k$ are $L^{n-1}mol^{1-n}s^{-1}=M^{1-n}s^{-1}$

Determining the Order of a Reaction

- Examine **initial rate** ($t=0$)
- Zeroth Order:
  - Concentration vs. Time: Linear
  - Rate vs. Time: Constant
- First Order
  - Initial Rate vs. Initial Concentration: Linear
- Second Order
  - Initial Rate vs. Initial Concentration: Quadratic
  - Initial Rate vs. Initial Concentration$^2$: Linear

Determination of rate laws from experimental data

- Determine the order of reaction for each reactant and the overall order
- When comparing concentration and initial rate, look for the same concentrations
- $k = \frac{v}{[A]^a[B]^b[C]^c...}$

Pseudo Order of Reaction

- The concentration of one reactant is significantly higher than other reactants, throughout the reaction, the concentration of this reactant will be almost constant
- $v=k[S_2O_8^{2-}][I^-] \approx k'[I^-]$, if persulfate's concentration is $100$ times higher than that of iodide ions
- Turned a second-order reaction into a *pseudo* first-order reaction with a *pseudo* first-order rate constant: $k'=k[S_2O_8^{2-}]$

Integrated Rate Laws

- 1st Order IRL ($aA \to B$)
  $$
  v=-\frac{1}{a}\dv{[A]}{t}=k[A] \to \frac{\dd {[A]}}{[A]}=-ak\cdot \dd t
  $$

  $$
  \int_{[A]_0}^{[A]} \frac{\dd {[A]}}{[A]} = -ak \int_0^t \dd t
  $$

  $$
  \int_{[A]_0}^{[A]} \frac{\dd{[A]}}{[A]} = \ln{[A]}-\ln{[A]}_0 = \ln(\frac{[A]}{[A]_0})=-akt
  $$

  $$
  \ln{[A]} = \ln{[A]}_0 - akt \to [A] = [A]_0e^{-akt}
  $$

- 0th Order IRL
  $$
  v=-\frac{1}{a}\dv{[A]}{t}=k \to \int_{[A]_0}^{[A]} \dd {[A]} = -ak \int_0^t \dd t
  $$

  $$
  [A] = [A]_0 -akt
  $$

- 2nd Order IRL
  $$
  -\dv{[A]}{t}=ak[A]^2 \to \frac{1}{[A]} = \frac{1}{[A]_0} - akt
  $$

Half-life of a reactant

- 0th Order: $t_{\frac{1}{2}} = \frac{[A]_0}{2ak}$
- 1st Order: $t_{\frac{1}{2}} = \frac{\ln2}{ak}$
  - Forms the basis for radiocarbon dating
  - $^{14}_6C \to ^{14}_7N + \beta^- + \nu$
- 2nd Order: $t_{\frac{1}{2}} = \frac{1}{ak[A]_0}$

Consecutive Reactions

- $A \xrightarrow{k_1} B \xrightarrow{k_2} C$
- $-\dv{[A]}{t} = k_1[A], \dv{[B]}{t}=k_1[A] - k_2[B], \dv{[C]}{t} = k_2[B]$
- If $k_1 << k_2$, $[B]$ never gets a chance to build up, then we can treat the system as $A \xrightarrow{k_1} C$
- Steady State: $\dv{[X]}{t} = 0$

Parallel Reactions

- $A + B \xrightarrow{k} C + D, A + B \xrightarrow{k^*} E + F$
- $v = -\dv{[A]}{t} = k[A][B] + k^*[A][B] = (k+k^*)[A][B] = k_{sum}[A][B]$
- The most rapid path determines the predominate path

Equilibrium

- $A \rightleftharpoons B$
- At equilibrium, $k_f[A] = k_r[B] \to \frac{[B]}{[A]} = \frac{k_f}{k_b} = K_{eq}$

### Reaction Mechanism

- Most reactions occur by a series of steps
- A reaction mechanism is a step-by-step description of a reaction
- The rate law can be determined from the reaction mechanism
- **Rate determining step** and **Steady state approximation**

Temperature Dependence of Reaction Rates

- Arrhenius Equation: The rate constant is a function of temperature

$$
\ln k = \ln A - \frac{E_a}{RT} \leftrightarrow k = Ae^{-\frac{E_a}{RT}}
$$

- $A$: pre-exponential factor (same unit as $k$), $E_a$: activation energy

$$
\ln(\frac{k_1}{k_2}) = -\frac{E_a}{R}(\frac{1}{T_1}-\frac{1}{T_2})
$$

Interpretation of Arrhenius Law

- Assumptions
  - Molecules or atoms must collide to react ($A$)
  - The collision must provide enough energy ($E_a$)
- Three questions (Gas phase reaction of $O_2$ molecules at $300K$)
  - Speed of the molecule
    - $v_{rms} = \sqrt{\frac{3RT}{M}} = 484 m/s$
    - $\bar{c} = 630 m/s$
  - Cross section
    - $\sigma \approx 1.8 \times 10^{-19} m^2/molecule$
  - Concentration
    - $[O_2] = \frac{PN_A}{RT} = 2.45 \times 10^{25} molecules / m^3$
  - $\bar{c} \sigma [O_2] = 2.8 \times 10^9 collisions \cdot s^{-1}$
  - Rate of collision: $\frac{\bar{c} \sigma [O_2]^2}{2} = 3.4 \times 10^{34} collisions \cdot m^{-3} \cdot s^{-1}$
  - $v = k[O_2] = Ae^{-\frac{E_a}{RT}}[O_2]^2 = \frac{\bar{c} \sigma [O_2]^2}{2} e^{-\frac{E_a}{RT}}$
  - $A = \frac{\bar{c}\sigma}{2}$
- Collision Theory
  - Fraction of molecules $f$ that collide with a kinetic energy that is no less than $E_{min} \approx E_a$ for a reaction is given by the shaded areas under each curve
  - $f \approx e^{-\frac{E_{min}}{RT}}$
  - Boltzmann distribution
  - $A$ is roughly constant
  - $P$ is fudge factor: effective collision factor

Elementary Reactions

- The rate law of an elementary reaction can be determined without an experiment
- Unimolecular: $v = k[A]$
- Bimolecular: $v = k[A]^2$ or $v = k[A][B]$
- Termolecular (**very slow**): $v = k[A][B][C]$, $v=k[A]^2[B]$, $v = k[A][B]^2$, or $v = k[A][B][C]$

### Steady State Approximation

- List rate laws for each step of reaction
- Identify the intermediate and find the expression the rate of change
- Find the concentration of the intermediate in terms of concentration of reactants, products, and rate constants
- Substitute the concentration of the intermediate to the proper rate expression
- Final rate law must not include intermediates

### Catalysis

- Accelerates or decelerates the reaction but undergoes no net chemical change
- Provide new pathway with a lower activation energy
- Enzymes
  - Homogeneous catalysts that catalyze reactions necessary to life
- Substrate
  - Molecules on which the enzymes act to promote biochemical reactions
- Michaelis-Menten mechanism
  - $E + S \rightleftharpoons ES \to E + Product$
  - Three steps, three rate laws, Steady State Approximation to find the general rate law
  - $v_r = \frac{v_{max}[S]}{K_M + [S]}$
    - $v_{max} = k_3 [E]_{total}$
    - $K_M = \frac{k_2 + k_3}{k_1}$
    - when $v = \frac{1}{2}v_{max}, K_M = [S]$
- Alternative form of the Michaelis-Menten Equation - Lineweaver-Burke Equation
  - $\frac{1}{v_r} = \frac{K_M}{v_{max}} \frac{1}{[S]} + \frac{1}{v_{max}}$
  - $y=mx+b$
    - $y = \frac{1}{v_r}$
    - $x = \frac{1}{[S]}$
    - $m=\frac{K_M}{v_{max}}$
    - $b = \frac{1}{v_{max}}$

## Quantum Chemistry

- Chemistry based on interaction of atoms

  - *electrons are the key in bonding*

- Probe: ***electromagnetic radiation***

  - An oscillating electric field

  - Associated perpendicular magnetic field
    $$
    c = \nu \lambda
    $$

    $$
    E = h \nu = \frac{hc}{\lambda}
    $$

- Why Quantum Mechanics

  - Black Body Radiation

    - Different atoms and molecules can emit or absorb energy in discrete quantities only

    - The amount of energy is "quantized"
      $$
      \hbar = \frac{h}{2 \pi}
      $$

      $$
      \lambda_{max} \approx \frac{hc}{4.965kT} = \frac{2.9 \times 10^{-3}}{T}m
      $$

  - Photoelectric Effect

    - Light exists as small packets of energy now known as photons

  - Optical Line Spectra
    $$
    \frac{1}{\lambda} = Z^2 R_H (\frac{1}{n'^2} - \frac{1}{n^2})
    $$

    - $R_H: 1.09677 \times 10^7 m^{-1}$
    - $n'<n$

- Bohr Model

  - $mvr = \frac{nh}{2\pi}$
  - $e^-$ travel in perfectly defined orbits around the nucleus
  - Energy is quantized
  - Excellent at predicting energy of one-electron species
  - $R_H = \frac{m_e e^4}{8 \epsilon_0^2 h^3c}$
  - $E = -\frac{m_e e^4}{8 \epsilon_0^2 h^2} \frac{Z^2}{n^2} Joules$
    - $\frac{m_e e^4}{8 \epsilon_0^2 h^2} = 2.1795 \times 10^{-18} Joules$
    - $E = -\frac{1}{2} \frac{Z^2}{n^2} Hartree$
    - Only applies to one electron species
  - Atomic units are the best to do quantum mechanics

- Particle/Wave Duality

  - Any small particles of matter may at times display wavelike properties

  - de Broglie Equation
    $$
    \lambda = \frac{h}{p} = \frac{h}{mv}
    $$

- Heisenberg Uncertainty Principle
  $$
  \Delta x \Delta p \ge \frac{h}{4\pi}, \Delta E \Delta t \ge \frac{h}{4\pi}
  $$

  - It is impossible to simultaneously measure both the *position* and *momentum* of a subatomic particle

- Schrodinger Equation (Time-Independent)
  $$
  \hat{H}\Psi = E\Psi
  $$

  - $\Psi$: wavefunction
    - for confined $e^-$ are standing waves
  - $\hat{H}$: Hamiltonian operator

- Particle In a Box

  - Probability $\propto \Psi^2$

  - Normalized wavefunction
    $$
    \int_0^l \psi_n(x)\psi_n^*(x)\dd x = 1
    $$

  - Possible values of $\lambda = \frac{2l}{n}$

  $$
  -\frac{\hbar^2}{2m}\dv[2]{\psi}{x} + U(x)\psi = E\psi
  $$

  $$
  \hat{H} = -\frac{\hbar^2}{2m}\dv[2]{x}
  $$

  $$
  \psi = \sqrt{\frac{l}{2}}\sin(\frac{n\pi x}{l})
  $$

  - Energy of a Particle in a Box
    $$
    E_K = \frac{n^2h^2}{8ml^2}
    $$

- What is a wavefunction?
  - Electron is described by a wavefunction
  - Phase of the electron's wavefunction changes at each node
  - Probability of finding the electron at a particular point $x$ is proportional to $\psi^2$
  - Probability of finding the electron at a node is zero

### Electrons in Atoms

- Atom: 3D box

  - $e^-$ constrained in 3 dimensions
  - defined by interaction between $e^-$ and nucleus
  - $e^-$ will have both *kinetic* and *potential* energy

- Cartesian coordinates ($x, y, z$) vs. Spherical coordinates ($r, \theta, \phi$)

  - $\theta$: angle from $z$-axis - latitude
  - $\phi$: angle from $x$-axis in $xy$ plane - longitude

- Wavefunctions are called **orbitals**

  - In atomic units
    $$
    \hat{H} = -\frac{1}{2} \nabla^2 - \frac{Z}{r}
    $$

    $$
    \psi_{1,0,0} = \frac{1}{\sqrt{\pi}}e^{-Zr}
    $$

  - Orbitals are defined by 3 quantum numbers
    - Principal ($n = 1,2,3,...$)
    - Orbital Angular Momentum ($l = 0, 1, ..., n-1$)
    - Magnetic: ($m_l = -l, -l+1,...,0,..., l-1,l$)
    - $\psi_{n,l,m}$
  - For $H$, all orbitals with same principal value have the same energy (degeneracy)

- Atomic orbitals

  - Same $n$: same principal shell
  - Same $l$ within $n$: same subshell
    - The # of subshells = $n$
    - $s,p,d,f$
  - Orbitals have 3 parts: Radial part, angular part, constant
  - Increased distance from nucleus (exponential decay)
  - Presence of radial nodes (oscillatory part)

- Drawing atomic orbitals

  - Each type of subshell ($l$) has a specific **base shape**
  - Total # of nodes = $n-1$
    - Total # of angular nodes = $l$, they are planar
    - Total # of radial nodes = $n-l-1$, they are spherical
    - Node represents a change of phase in the wavefunction

- Electron spin facts

  - electron spin is quantized
  - $4$th quantum number: $m_s = \pm \frac{1}{2}$
  - $m_s$ does not depend on the previous three quantum numbers
  - Electron spin must be taken into consideration when "filling" orbitals
  - Consequence of the union of quantum mechanics and relativity
  - *electrons* are "fermions", all fermions have a half integer spin

- Multi-electron atoms

  - repulsion between electrons

  - higher $Z$ =  lower orbital energies

  - shape/size of orbitals is not the same

  - orbitals with same $n$ do not have same energy

  - Helium

    - Need approximations, no analytical solution

  - Perturbation theory

    - modify the Hamiltonian operator
      $$
      E = E^{(0)} + E^{(1)} + ... \leftrightarrow \hat{H} = \hat{H}^{(0)} + \hat{H}^{(1)}+...
      $$

  - Variational method

    - Set and change parameters until a minimum energy is reached
      $$
      E_0 \le \frac{\int \psi \hat{H} \psi \dd \tau}{\int \psi^2 \dd \tau}
      $$

- 

- Electronic Configurations
  - Start with ground state
  - Pauli exclusion principle
    - Two electrons in an atom **may not** have the same quantum numbers
  - Aufbau process
    - Building up based on energy ordering of atomic orbitals
  - Hund's rule
    - Electrons in different singly occupied orbitals of the same subshell have the same or parallel spins
    - Higher total spin = lower energy
- Periodic Table
  - Only outer (valence) electrons take part in chemical reactions and bonding
  - Outer-shell electron configuration determines chemistry
  - Periodicity in outer-shell electron configuration shown by periodic table
  - Periodic Trends
    - Ionization energies
      - Energy required to remove an electron from an atom
      - Half-filled and filled shells are stable
      - Across a row increases
      - Down a group decreases
    - Effective charge ($Z_{eff}$)
      - Increases down a group because the screening by inner-shell electrons is not perfect
      - Increases across a row, but less than expected because of screening by other valence electrons
    - Atomic radius
      - Along a row, size decreases
        - Greater nuclear charge
        - No screening in same level
      - Down a group, size increases
        - Outer electrons are in levels with greater $n$
    - Reactivity
      - Group 1 - alkali metals
      - Group 17 - halogens
    - Metallic Character
      - Most metallic, bottom left
      - Least metallic, top right

## VBT and MO Theory

- Covalent bonds are molecular orbitals: constituted by atomic orbitals overlapping

### Valence Bond Theory

- Atomic orbitals combine and mix: hybridized atomic orbitals
- $1 \times 2s + 3 \times 2p = 4 \times sp^3, 3 \times sp^2 + 1 \times p, 2 \times sp + 2 \times p$
- Same hybridization = same size, shape, energy; not the same geometry
- Total Energy of 4 hybridized orbitals = Total Energy of 4 original atomic orbitals
- Linear combination of atomic orbitals
  - $sp^3$: $75\%$ p-character, $sp$: $50\%$ p-character,...
- Electrons are held farther from the nucleus in the order $sp^3 > sp^2 > sp$
- Geometry
  - $sp^3$: Tetrahedral
  - $sp^2$: Trigonal planar
  - $sp$: Linear
- Bonds (molecular orbitals)
  - $\sigma$ bond: $s-s (sp^n)$ bonding, formed by atomic orbitals pointing toward each other, electron density around and between the nuclei
  - $\pi$ bond: $p-p$ bonding, electron density above and below the axis containing the $\sigma$ bond, parallel but close enough to overlap, **overlap of all 4 lobes**
  - Normally, cannot have $\pi$ bond without a $\sigma$ bond
- Determining hybridization
  - $0 \times p = sp^3$
  - $1 \times p = sp^2$
  - $2 \times p = sp$
- Conjugation
  - If an atom **can** be **conjugated** to a $\pi$-system, it **will** be. Thus that atom will be considered to have at least one (unhybridized) p-orbital

### Molecular Orbital Theory

- Molecular orbitals can be bonding (energy of MO $<$ AOs), non-bonding (energy of MO $=$ AOs), or anti-bonding (energy of MO $>$ AOs)

$$
Bond \space Order = \frac{(bonding \space e^-)-(antibonding \space e^-)}{2}
$$

- Bonding: In phase; Anti-bonding: Out of phase
- $e^-$ filled into MOs as they are in AOs, low energy first, no more than 2 per orbital, opposite spin
- $\sigma$ bonds are composed of AOs that point toward each other; $\pi$ bonds are composed of AOs that are parallel to each other; $p$ orbitals can form $\sigma$ bonds in MO theory
- As $Z$ increases, the energy levels between $2s$ and $2p$ are farther apart
  - $B$: $2s$ and $2p$ orbitals can mix
  - $Ne$: $2s$ and $2p$ orbitals cannot mix
  - Energy levels of the elements will change
- Magnetism
  - Diamagnetic: No unpaired electrons, lightly repelled by a magnetic field
  - Paramagnetic: Has unpaired electrons, attracted to a magnetic field
- HOMO: Highest Occupied Molecular Orbital; LUMO: Lowest Unoccupied Molecular Orbital
- $\pi$-Delocalization
  - Conjugated system (all atoms in the chain must have a $p$-orbital in the same plane)
  - Butadiene: four $2p$ AOs combine to form 4 $\Psi$ MOs
  - Allylic system: allylic cation, radical, and anion are all stabilized due to delocalization
  - Delocalization requires the $p$-orbitals to be contiguous and coplanar
  - **Allene**: is not conjugated because $p$-orbitals are not co-planar
- Resonance
  - Charge delocalized is more stable than charge localized
  - Curved arrows to indicate electrons movement
  - Reason
    - Polarity of carbonyl
      - Electronegativity
      - Charge on $C$, $O$ from resonance
  - Missing an octet is worse than placing $+$ charge on a more electronegative atom
  - The only time we use chare separation in resonance structures is to demonstrate such polarity and certain bond characters; we do not use charge separation in a simple alkene nor a simple benzene ring
  - Formal charges
    - To minimize the number of formal charges
    - To minimize the number of atoms lacking an octet
    - No second row atom should have a formal charge other than 0, +1, or -1
- What drives conjugation
  - Small energetic cost in promoting an orbital from $sp^3$ to $p$, but there is a large energetic payback through conjugation
- Inductive effects
  - Depends on electronegativity, draws $e^-$ density
  - $O$, $N$: donate to the $e^-$ density more than draw from it
  - $F$: draws from $e^-$ density more than donate to it

## Acid-Base

Bronsted-Lowry

- Acid: Donates $H^+$
- Base: Accepts $H^+$
- Conjugate acid-base pair

Lewis

- Acid: Accepts $e^-$ pair
- Base: Donates $e^-$ pair

$$
HA + H_2O \rightleftharpoons A^- + H_3O^+
$$

$$
K_a = \frac{[H_3O^+][A^-]}{[HA]}, pK_a = -logK_a
$$

Dissociation constant

- Strong acids: $K_a >> 1$, dissociation is nearly complete
- Weak acids: $K_a < 1$, dissociation is incomplete
- Equilibrium constant for water dissociation is $K_w = 10^{-14}$ at $25^{\circ}C$
- $K_a K_b = K_w$, for any conjugate acid-base pair

$$
pH = -log[H_3O^+], [H_3O^+] = 10^{-pH}
$$

$$
pOH = -log[OH^-], [OH^-] = 10^{-pOH}
$$

- The smaller the $pK_a$, the stronger the acid
- The smaller the $pK_b$, the stronger the base
- The salt of a weak acid gives a basic solution, the salt of a weak base gives an acidic solution

### Buffers

- Solutions that are resistant to changes in $pH$ upon addition of water, acid, or base
- Weak acid $+$ its conjugate base in "appreciable amounts"
  - Equimolar of acid + base $\to$ $pH = pK_a$

$$
[H_3O^+] = 10^{-pH} = K_a \frac{[HA]}{[A^-]}
$$

### Organicky Acid-Base Chemistry

- Conjugate base of a strong acid is a weak base
- Conjugate base of a weak acid is a strong base
- Equilibria will always lie toward the weaker (more stable) acid and base

$$
ROH + R'CO_2^- \rightleftharpoons RO^- + R'CO_2H
$$

$$
K = \frac{[RO^-][R'CO_2H]}{[ROH][R'CO_2^-]} = \frac{K_a(ROH)}{K_a(R'CO_2H)}
$$

- charges are unstable
  - Charge stabilization: negative charge on  a conjugate base; positive charge on a conjugate acid
- Electronic effects on $pK_a$
  - More electronegative atoms can hold a negative charge better (basicity decreases as you go to the right in the same row)
  - Basicity goes up as you go up on the Periodic Table: larger atoms can hold a negative charge better since the charge is more spread out in a much larger orbital
  - Resonance: the more stable of a conjugate base, the stronger is the conjugate acid
  - Inductive effects: More electronegative atoms can stabilize a negative charge through one or more $\sigma$-bond via "induction"
  - Hybridization and Bonding: negative charge closer to the nucleus is more stable, thus more $s$-character, more stable
    - Carboanion: $sp^3 < sp^2 <sp$
  - Hydrogen bonding: Intramolecular hydrogen bonding is more stable
  - Aromaticity: If protonation of a molecule breaks up its aromaticity (6 $\pi$ electrons), then the resulting compound will be highly acidic. The original molecule will be stable and non-basic

### $\alpha$-amino acid

- amino group: basic
- carboxyl group: acidic
- In steps of dissociation: the most acidic proton dissociates first
- Why is the $pK_a$ of the carboxylic acid of an $\alpha$-amino acid so much lower than that of acetic acid
  - Inductive effect: positive charge on the ammonium a few bonds away inductively withdraws electron density from the carboxylate and thereby stabilizes the negative charge
- Isoelectric point
  - The pH at which the amino acid exists in solution predominantly as a neutral species

$$
pI = \frac{pK_a(1+)+pK_a(1-)}{2}
$$

## Substitution Reaction Mechanisms

### SN2 (Bimolecular nucleophilic substitution)

$$
CH_3Br + I^- \to CH_3I + Br^-
$$

- Bromomethane is **electrophile**: in the form of a lone pair of electrons to form a new covalent bond. Lewis acids. Electrophilic carbon has a partial positive charge due to the dipole of the polar covalent bond
- $I^-$ is **nucleophile**: donates a pair of electrons to an electrophile to form a new covalent bond. Lewis bases
- $Br^-$ is **leaving group**: leaves from electrophile
- $v = k[CH_3Br][Na^+I^-]$, obey second-order kinetics
- Carbon makes a new bond and breaks an old bond; it remains tetravalent
- Any of iodide's 4 lone pairs can attack
- Carbon is attacked from its "backside" (back lobe of the $C-Br$ bond)
- $C-Br$ bond is broken heterolytically, both electrons goes to $Br$, as opposed to homolytically
- During transition state, both iodide and bromide are partially bonded to carbon, each has a partial negative charge
- Electrophilic carbon is said to undergo **Walden Inversion**, where the substituents invert about the carbon
- It is concerted as the attack by the nucleophile and the departure of the leaving group occur in concert (simultaneously); there are no intermediates
- The rate of the SN2 reaction depends on
  - The structure of the electrophile
  - The nucleophilicity of the nucleophile
  - The stability of the leaving group
  - The polarity of the solvent
- Electrophile
  - Methyl structure: $CH_3 - X, v_{relative} = 30$
  - Primary ($1^{\circ}$) structure: $CH_3 - CH_2 - X, v_{relative} = 1$
    - Primary electrophiles cannot undergo SN1 reactions
  - Secondary ($2^{\circ}$) structure: $(CH_3)_2 - CH- X, v_{relative} = 0.02$
    - This electrophile can undergo either reaction
  - Tertiary ($3^{\circ}$) structure: $(CH_3)_3 - C - X, v_{relative} \approx 0$
    - Tertiary electrophiles do not undergo SN2 reactions
- Nucleophile
  - More polarizable **lone pairs** are better: polarizability refers to how easily the electron density in an orbital can be reshaped by a local charge or dipole
  - "Hard" orbitals: $O$, $N$; "Soft" orbitals: $S$, $P$
  - Conjugate bases are better nucleophiles than their conjugate acids
- Periodic Trends
  - Nucleophilicity increases as you go down the Periodic Table due to an increase in polarizability
  - Nucleophilicity increases as you go to the left of the Periodic Table due to decreased nuclear charge
  - Basicity increases as you go up the Periodic Table due to greater charge density (higher affinity for proton); Basicity increases as you go to the left on the Periodic Table due to lower electronegativity
- Leaving groups
  - Good leaving groups are those that are stable in solution with the pair of electrons they have secured.
  - They must also have weak $C-leaving \space group$ bonds
  - Hydride and most carbanions are highly unstable and will not be leaving groups
  - Protonation of the alcohol converted a poor leaving group into a good leaving group
  - Its ability correlates with its stability (the $pK_a$ of its conjugate acid)
- Solvents
  - Good solvents for SN2 are moderately polar (and aprotic), stabilizes the polar transition state
  - Too polar, solvate the nucleophile too well, hindering it from reaction
  - Highly polar solvents also enhance SN1 reactions. Such solvents are called **protic** solvents if they contain an (weakly) acidic hydrogen ($\delta^+$ on $H$). They can dissociate, and can donate a hydrogen bond
- Stereochemistry
  - No stereogenic centers: Achiral product
  - Has stereogenic centers but not at the electrophilic carbon: start with optically pure, produce optically pure
  - Electrophilic center is the only stereogenic center: optically pure gives optically pure
  - Several stereogenic centers (including the reaction center): optically pure gives optically pure

### SN1 (Unimolecular Nucleophilic Substitution)

- Rate is dependent on the concentration of the electrophile and **independent** of the concentration of the nucleophile
- Two-step mechanism
  - First, the leaving group leaves, yielding an **intermediate** called a carbocation (rate-limiting step)
  - Second, the nucleophile then attacks the carbocation from either side of the plane
  - If the electrophilic carbon was a stereogenic center, the product is a racemic mixture, the hybridization of the carbon passes from $sp^3$ to $sp^2$ and back to $sp^3$
- Electrophile
  - Methyl and primary carbocations will not form
  - Secondary carbocations will be slow to form
  - Tertiary carbocations will form readily
  - Great stability of the more substituted carbocations is due to an ability of the alkyl groups to donate electron density into the cationic center, namingly **hyperconjugation**
- Nucleophile
  - Nucleophilicity is not very important
  - SN1 reaction is often called solvolysis (nucleophile is often the solvent)
- Leaving group
  - Must be stable
- Solvent
  - Highly polar solvents are best because they stabilize the fully charged carbocation intermediate
  - Protic solvents are better than aprotic solvents, better at solvating anions
  - At secondary centers: protic solvents will enhance SN1 reactions, aprotic solvents will enhance SN2 reactions
  - SN1 will occur in aprotic solvents on tertiary centers
- Stereochemistry
  - If center is a stereogenic center: stereoisomers will be produced, enantiomers or diastereomers
  - If center is not a stereocenter: only one product will from
- Intramolecular ring closures to form $3-6$ membered rings is much faster than intermolecular reactions

### Other chemicals

- Vinyl/Aromatic halides ($sp^2$ carbons) do not undergo SN1 or SN2
  - SN2: too hindered
  - SN1: CC bond is unstable
- Allylic/Benzylic carbons can undergo SN1 reactions

### Secondary Center Competitions

- Deduce the type of reactions from
  - The optical activity of the product
  - The properties of the solvent

### General Guidelines

- Under acidic conditions, try to limit oxygen states to neutral and $+$ ($ROH_2^+, ROH$)
- Under basic conditions, try to limit oxygen states to neutral and $-$ ($RO^-, ROH$)



