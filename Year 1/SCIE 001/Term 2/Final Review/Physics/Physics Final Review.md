# <center>Physics Final Review</center>

## Waves

### Harmonic Motion (Newton's Second Law + Hooke's Law)

$$
m \dv[2]{x}{t}=-kx
$$

- Mass on a string

$$
x(t) = A\cos(\omega t + \phi)
$$

$$
v(t) = -v_{max}\sin(\omega t + \phi)
$$

$$
a(t)= -a_{max}\cos(\omega t + \phi)
$$

- Angular frequency: $\omega = \sqrt{\frac{k}{m}}=2\pi f = \frac{2\pi}{T}$, $\omega (rad/s), f(Hz)$

- $v_{max}=A\omega, a_{max}=A\omega^2$

### Transverse Waves

- Damping
  - Time constant: time to decay to $\frac{1}{e}$ of the starting amplitude
  - Damping envelope: $A_0 e^{-\frac{t}{\tau}}, \tau=\frac{b}{2m}$
  - Time constant can be approximated by the x-intercept of the derivative function at the beginning of the oscillation.
  - Large Damping
    - $b^2 < 4mk$: mass oscillates, slowly losing amplitude
    - $b^2 = 4mk$: "critical damping", fastest return to equilibrium
    - $b^2 > 4mk$: does not oscillate, attempt to return to equilibrium position

$$
m \dv[2]{x}{t} + b \dv{x}{t}+kx=0
$$

$$
x(t)=A_0 e^{-\frac{b}{2m}t} \cos(\omega t + \phi)
$$

$$
\omega = \sqrt{\frac{k}{m}-(\frac{b}{2m})^2}
$$

- Forced Oscillation and Resonance
  - Natural vibration frequencies can excite system into motion more easily if the frequency is the same
  - $\omega$: Driving angular frequency
  - $\omega_0$: Natural angular frequency
  - For maximum amplitude: $\frac{b}{2m}=\frac{1}{2}\omega_0, \frac{1}{4}\omega_0, \frac{1}{8}\omega_0$
  - Quality Factor: $Q = \frac{\omega_0}{\Delta \omega} = \frac{m\omega_0}{b}$, $\Delta \omega$ is full width at half the maximum amplitude, or "half-height" (FWHM / FWHH)

$$
-kx - b \dv{x}{t} + F_0 \sin(\omega t)=m \dv[2]{x}{t}
$$

$$
x(t) = A \cos(\omega t + \phi)
$$

$$
A = \frac{F_0}{\sqrt{m^2(\omega^2-\omega_0^2)+b^2 \omega^2}}
$$

- Waves (Transverse)

  - Waves on strings (transverse + visible)

  - "Transverse" means the direction of the disturbance is at $90^{\circ}$ to the wave direction (Disturbance moves up and down, but wave travels to the left or right)

  - $v = \frac{\lambda}{T}=\lambda f$

  - String tension drives the wave (higher tension, higher velocity)

  - Angle & Position: $\frac{\theta}{x}=\frac{2\pi}{\lambda}$

    - At a given time: $y(x)=A\sin(\frac{2\pi}{\lambda}x)$
    - Position moves $vt$ in $t$

    $$
    y(x, t)=A\sin(\frac{2\pi}{\lambda}(x \pm vt))=A\sin(\frac{2\pi}{\lambda}x \pm 2\pi f t)
    $$

    $$
    y(x,t)=A\sin(kx \pm \omega t), k = \frac{2\pi}{\lambda}, \omega = 2\pi f
    $$

    - $+$: travelling to the left, $-$: travelling to the right
    - Speed of the wave: $v=\frac{\omega}{k}$

  - Reading a History Graph and a Snapshot Graph

    - History Graph: Information about direction of the wave  and $T$
    - Snapshot Graph: Information about $\lambda$
    - Combination gives information about $v, k, \omega$

### Standing and Longitudinal Waves

- Speed of waves on a string
  - $v=\sqrt{\frac{T}{\mu}}$, $\mu$: Linear density ($kg/m$)
- Standing waves (Incident + Reflecting waves = Nowhere wave)
  - $y_+ = A\sin(kx-\omega t)$, $y_- = A\sin(kx+\omega t)$
  - $y_+ + y_- = 2A\sin(kx)\cos(\omega t)$ (Prosthaphaeresis)
  - Nodes: no wave motion
  - Antinodes: maximal motion
  - Wavelengths: $\lambda_n = \frac{2L}{n}, \forall n \in \Z^+$, $L$ is the length of the string
  - Frequencies: $f_n = \frac{nv}{2L}, \forall n \in \Z^+$
    - Increase: Tension increase, Length decrease, Thickness decrease, Density decrease
    - Decrease: Length increase, Thickness increase, Density increase
- Longitudinal Waves
  - Displacements in the direction as that of the wave
  - Pressure (density) nodes and Displacement (velocity) nodes: pressure antinode $=$ displacement node, pressure node $=$ displacement antinode

### Pipes and Voice

- Infinite number of standing waves $\leftarrow$ open / close ends
  - Close end: Velocity node + Pressure antinode
  - Open end: Velocity antinode + Pressure node
  - Normal mode: A standing wave in which all parts of the object are moving with one frequency
    - Mode 2: An octave higher
    - Mode 3: $1.5$ octaves higher
- OPEN-OPEN tube

$$
\lambda = \frac{2L}{n}, f = \frac{nv}{2L}, \forall n \in \Z^+
$$

- CLOSE-OPEN tube (vocal tract)

$$
\lambda = \frac{4L}{n}, f=\frac{nv}{4L}, n=2k-1, \forall k \in \Z^+
$$

### Beats and Scales

- Beating occurs regularly with a frequency equal to the difference of the two frequencies contributing (two tones close together)

$$
f_{beat}=|f_2 - f_1|
$$

- Scales (see notes): Just temperament and Equal temperament

### Doppler Effect

- Refraction
  - Waves bend toward regions of lower wave speed (denser/colder air)
- Doppler effect
  - $\lambda_{observer}=\lambda_{source}(\frac{v-v_{source}}{v}), f_{observe} \approx f_{source}(1+\frac{v_{source}}{v}), v_{source} << v$
  - $\Delta f=|f_{observer}-f_{source}|=\frac{v_{source}}{v}$

$$
\frac{\Delta f}{f} \approx \frac{(2)v_{relative}}{v}
$$

- $2$ is for a passing vehicle
- Travelling faster than the wave speed
  - Shockwave
  - Faster than local speed of light (Cherenkov radiation) - Cherenkov cone
- Kelvin wakes ($39^{\circ}$)

### Noise and Waveforms

- Sound Intensity ($I$): $\propto$ acoustic pressure squared

$$
\beta(dB)=10\log_{10}(\frac{I}{I_0}), I_0=10^{-12}W/m^2(20 \mu Pa)
$$

- Sensitivity is frequency dependent
  - Phon: psychoacoustic quantity
  - phon $=$ $dB$ at $1000 Hz$
- Pluck a string (real modes)
  - The shape of the wave starts as triangular $=$ $\sum$ normal modes in different quantities (Fourier analysis)
  - Real waveforms $=$ Superposition of harmonics
  - Harmonic frequencies with a node at the position where the string is plucked will **NOT** contribute to the superposition

### Interference and Diffraction

- Continuous waves can be summed to an isolated pulse

- Waves $\leftrightarrow$ Particles

  - $p_{particle} \propto k$, $k=2\pi n$ (wavenumber)
    $$
    p=\hbar k
    $$

  - $E_{particle} \propto f$
    $$
    E=hf=\hbar \omega
    $$

  - Heisenberg's Uncertainty Principle
    $$
    \Delta p \Delta x \ge \frac{h}{4\pi}, \Delta E \Delta t \ge \frac{h}{4\pi}
    $$
    

- Interference

  - Constructive Interference: $2$ crests: bigger crest, $2$ troughs: bigger trough
    $$
    \Delta x_{total} = \Delta x_{path} + \Delta \phi=n\lambda
    $$

  - Destructive Interference: crest $+$ trough = cancellation
    $$
    \Delta x_{total} = \Delta x_{path} + \Delta \phi=(n+\frac{1}{2})\lambda
    $$

  - In phase ($\Delta \phi = 2\pi n$)

    - Constructive: $\Delta x=n\lambda$
    - Destructive: $\Delta x = (n+\frac{1}{2})\lambda$

  - Out of phase / In anti-phase ($\Delta \phi = (2n+1)\pi$)

- Diffraction

  - Wave encounters an object of similar or smaller size than its own wavelength ($\lambda_{wave} \ge \lambda_{object}$)
  - Larger difference, larger spread; Smaller difference, smaller spread
  - Huygen's Principle

## Quantum Mechanics

### Young's Double Slit Experiment

$$
\Delta r=n\lambda
$$

$$
\frac{\Delta r}{d} \approx \frac{y}{L}
$$

​	$d$ is the distance between the slits, $y$ is the distance from the midline to the $n$th bright fringe, $L$ is the distance between the slits and the screen
$$
\Delta y= \frac{\lambda L}{d}
$$

### Wavefunction

- Ultraviolet catastrophe

- Photoelectric effect

  - Do work on conduction electrons in metal such that they gain high enough kinetic energy to escape metal

  - Minimum energy required is called "work function"

  - Electromagnetic radiation is quantized
    $$
    E=hf
    $$

  - Light comes in chunks (discrete "quanta")

  - *Power* of a light source is related to the number of photons the light emits times the energy per photon
    $$
    P=\dv{E_{light}}{t}=\dv{N}{t}hf
    $$

  - Superposition of huge numbers of photons behave like a classical wave

- Double slit experiment with one photon

  - Initial state only determines the **PROBABILITIES** for various outcomes
  - This probability matches intensity pattern from the electromagnetic wave

- de Broglie: Matter can behave as a wave

  - Interference pattern follows **de Broglie wavelength**
    $$
    \lambda=\frac{h}{p}=\frac{h}{mv}, f=\frac{E}{h}
    $$
    
  - $I(x) \propto |A(x)|^2$, $I$ is the intensity of the electromagnetic wave, and $A$ is the amplitude of the electromagnetic wave
  
- Wavefunction model ($\Psi (x,t)$)

  - $|\Psi(x,t)|^2$ tells us the **PROBABILITY DENSITY** of finding a particle at $x$ if we measure it $\rightarrow$ defines a quantum superposition

$$
\int_{-\infty}^{\infty} |\Psi(x)|^2 \dd x=1
$$

$$
P(x_1, x_2)=\int_{x_1}^{x_2} |\Psi(x)|^2 \dd x
$$

### Wave Packets

- Wavefunction has complete information about the physical configuration "state" of the system
- One wavefunction describes one particle
- Wavefunction $=$ $\sum$ position eigenstate or $\sum$ momentum eigenstate
- Eigenstate
  - Measurement: dynamic process in which the wavefunction undergoes a drastic change
    - Irreversible interaction with a quantum system
    - Observables: measured system properties
    - Defined mathematically by "operators"
    - Wavefunction immediately after a measurement $\rightarrow$ Eigenfunction/Eigenstate of the operator associated
  - Position eigenstate: a measurement of position is made, wavefunction collapses
    - Wavefunction: spread out $\rightarrow$ localized
  - Momentum eigenstate ($p=\frac{h}{\lambda}$)
    - Definite momentum: pure sinusoidal wave with definite wavelength
- Wave packet
  - Real travelling particles $=$ wave + particle
  - Wavefunction $=$ Wave packet
  - Wave packet: localized like a particle (expect to find within $\Delta x$, width of "wave packet"), clear wavelength
  - Spatial extent $\ge$ $\lambda$
  - Minimum range of non-zero position
  - Knowing smth about momentum limits how certain we are about position
  - Wave packet $=$ Superposition of eigenstates
    - Each eigenstate has a definite "**observable**" quantity associated with it

### Heisenberg's Uncertainty Principle & Schrodinger's Equation

- Wave packet represents a traveling particle, moves with speed
  $$
  v=\frac{h}{m \lambda}
  $$

- $\lambda$ in wave packet matches the $\lambda$ of pure wave that contributes the most to superposition (*technically matches $\bar{\lambda}$*) $\leftrightarrow$ Fourier Decomposition

  - A single pure wave defines a single momentum eigenstate (perfectly defined $p$, completely unknown $x$)

$$
\Delta x \Delta p \ge \frac{h}{4\pi}
$$

- Wavefunction as time progresses
  - If moving to the right
    - Much wider than it was before (more uncertain of the particles position) (spreads out)
    - Smaller $\lambda$ at the front (right) and larger $\lambda$ at the back (left)
    - Higher momentum eigenstates move faster than lower momentum eigenstates
- $x$ and $p$ are incompatible observables: One cannot know the value of incompatible observables simultaneously with arbitrary precision
- Speed of spreading out?
  - Smallest $\Delta x$ $\rightarrow$ Largest $\Delta p$, greater speed in velocities of momentum eigenstates that make up the packet
- Schrodinger-ish Equation (with no force)
  - pure sinusoidal waves

$$
\dv{\Psi}{t}=(const.)\frac{1}{m}\dv[2]{\Psi}{x}
$$

- $\dv{\Psi}{t}$ is equivalent to frequency, $\dv[2]{\Psi}{x}$ is equivalent to $\frac{1}{m\lambda^2} \propto \frac{p^2}{m} \propto mv^2 \propto E$ (if no potential energy, $E = KE$)

$$
E=hf=\frac{p^2}{2m}, f=\frac{E}{h}
$$

- Euler Progression - How "fast" the wavefunction evolves depends on the energy of the particle

$$
\Psi(x, t + \delta t) = \Psi(x, t) + \delta t (const.)\frac{1}{m}\dv[2]{\Psi}{x}
$$

- Schrodinger-ish equation with constant $U$

$$
\dv{\Psi}{t}=(const.)\frac{1}{m}\dv[2]{\Psi}{x} + U \Psi
$$

$$
f=\frac{1}{h}(\frac{h^2}{2m\lambda^2}+U), hf=\frac{p^2}{2m}+U = E
$$

- Infinite Potential Well
  $$
  \lambda_n = \frac{2L}{n}=\frac{h}{mv} \rightarrow v_n = n \frac{h}{2Lm}
  $$

  $$
  E_{n}=\frac{n^2h^2}{8mL^2}
  $$

- Particles have quantized energies: standing waves

- Bound energy states exist for any "trapped" wavefunction with $E_{total}<U_{\infty}$(energy required to escape potential well)

## Electrostatics

### Introduction

- Charged objects can attract or repel each other; Charged objects can attract neutral objects
- Properties of electric charges
  - 2 types: + and -
  - Charge is quantized
  - Like charges repel, unlike charges attract
  - Charge is conserved
- Insulators: No freely mobile charges; Conductors: Freely mobile charges
- Polarization: One side of the atom gets more negative than the other
  - 2 opposite charges slightly separated form an "electric dipole"
  - Polarize Insulators/Conductors
  - Discharging: Conductors in contact share charges
  - Grounding: Connecting an object to the Earth
- Electroscope
  - Rotates away from vertical axis when charged object is brought near
- Electric force - Coulomb's Law ($\epsilon_0$: permittivity of free space)

$$
F = \frac{kq_1 q_2}{r^2}
$$

- Net force (superposition of forces) $=$ $\sum$ individual forces
- Electric Field
  - Physical quantity whose value is a function of position, relative to the source of the field
  - Vector field and Scalar field
  - Charges $=$ sources

$$
\vec{F}=q\vec{E}
$$

### Electric Fields

$$
\vec{a}=\frac{q\vec{E}}{m}
$$

- Charge-to-mass ratio is **critical**
- Intermolecular forces
  - London dispersion: Ubiquitous attractive forces that exist in **all** atoms & molecules
  - Dipole-dipole
  - Hydrogen bonding
  - Charge-dipole: Attractive force between an ion and the dipole of a polar molecule
  - Ion-Ion interaction
- Field of Point charge

$$
\vec{E}=\frac{kq}{r^2}\hat{r}
$$

$$
|\vec{E_p}|=E_p=\frac{kq}{r^2} [N/C]
$$

$$
\hat{r}=\frac{\vec{r}}{r}
$$

$$
\vec{F_{1 \to 2}}=\vec{F_{2 \to 1}}
$$

$$
\vec{E_p}=\sum_{i=1}^n \vec{E_i}
$$

### Fields of Various Charge Distributions

- Charge-Dipoles ($\vec{p}=qs$, $s$ is the length of the dipole)

$$
\vec{E}=\frac{2k\vec{p}}{x^3}
$$

- Dipole-dipole ($\vec{F} \propto \frac{1}{r^4}$)
- Torque on a dipole ($\vec{p}$ is pointing from $-$ to $+$, and $\vec{E}$ is the field of the charge)

$$
\vec{\tau}=\vec{p} \times \vec{E}
$$

- Continuous charge distributions

  - Linear Charge
    $$
    \lambda = \frac{Q}{L}
    $$

    - If $d >> L$, $\vec{E} = \frac{kQ}{d^2}$
    - (Infinite Line of Charge) If $L \to \infty$, $\vec{E}=\frac{2k \lambda}{d}$

  - Planar Charge
    $$
    \sigma = \frac{Q}{A}
    $$

  - Volumetric Charge
    $$
    \rho = \frac{Q}{V}
    $$

  - $d\vec{E} \leftrightarrow d\vec{q}$

### Fields and Potentials

- Infinite Line of Charge: see above

- Infinite Plane of Charge

  - The strength of the electric field is not related to the distance between the charge and the plane

- Symmetry

  - Charge distribution is *symmetric* if there is a group of *geometric transformation* that does not causer any *physical change*

  - Translation, Rotation, Reflection

  - **Symmetry of the electric field must match the symmetry of the charge distribution**
    $$
    E_{sphere}=\frac{kQ}{r^2}, E_{line}=\frac{2k\lambda}{r}, E_{plane}=\frac{\sigma}{2\epsilon_0}
    $$

- Capacitor: Two planes of equal, opposite charges
  $$
  E = 2E_{plane}=\frac{\sigma}{\epsilon_0}=\frac{Q}{A\epsilon_0}
  $$

- Quadrangle of Electrostatics

  - Force $\leftrightarrow$ Potential Energy
    $$
    F_s = -\dv{U}{s}, \Delta U= \int_i^f \vec{F} \cdot \dd {\vec{s}}
    $$

  - Electric force = conservative force
    $$
    \vec{F} = \frac{kq_1 q_2}{r^2} \hat{r}, U=\frac{kq_1 q_2}{r}
    $$

### Potentials and Conductors

- Quadrangle of Electrostatics
  $$
  U_{total}=\sum_{i<j}^N U_{ij}=\sum_{i<j}^N \frac{k q_i q_j}{r_{ij}}
  $$

  - Potential Energy $\leftrightarrow$ Electric Potential
    $$
    U=qV, V = \frac{U}{q}= \frac{kq}{r}
    $$

  - Electric Field $\leftrightarrow$ Electric Potential
    $$
    E_s = -\dv{V}{s}, \Delta V = -\int_i^f \vec{E} \cdot \dd{\vec{s}}
    $$

- Topographic Maps for Electrostatics
  - Equipotential line: a line of constant electric potential
    - Closer equipotential lines means stronger electric field
  - Saddle point (The change in electric potential is zero, electric field is zero)
  - Electric field lines are perpendicular to the equipotential surfaces and point "downhill"
- The electric field in a conductor in electric static equilibrium is zero.
  - $E=0$ in a conductor implies that the **entire conductor is an equipotential**, thus the E-field must be perpendicular to the surface

## Circuits (Kirchhoff's Law)

### Resistors, Batteries and Power

$$
R = \frac{V}{I}
$$

Series
$$
R_{eq}=\sum_{i=1}^N R_i
$$
Parallel
$$
\frac{1}{R_{eq}} = \sum_{i=1}^N \frac{1}{R_i}
$$
Power
$$
P=IV=\frac{V^2}{R}=I^2 R
$$
Batteries - $r$ is internal resistance, $I = \frac{\epsilon}{r+R}$, maximum power when $r=R$ (power is half-half split)
$$
V=\epsilon - Ir
$$

- $I_{max}=\frac{\epsilon}{r}$
- $V_{R_{max}}=\epsilon$

### Capacitors, Non-Linear Components

Capacitance of a parallel-plate capacitor - Farads $[C/V]$
$$
C = \frac{Q}{V} = \epsilon_0 \frac{A}{d}
$$

- RC circuits ($\tau = RC$)

  - Charging a capacitor
    - Capacitor: Charge increases, Voltage increases
    - Resistor: Current decreases, Voltage decreases
  - Discharging a capacitor
    - Capacitor: Charge decreases, Voltage decreases
    - Resistor: Current decreases, Voltage decreases

- Energy in electric field

  - Energy density in electric field

  $$
  u_{E} = \frac{1}{2}\epsilon_0E^2
  $$

  - Energy stored in capacitor

  $$
  U_C = \frac{1}{2}V^2C = \frac{1}{2}QV
  $$

- Electron states in solids
  - Band gap between Valence Band and Conduction Band
  - "Doping"
    - Internal electric field can be generated $\rightarrow$ Diode will allow current to pass one way but not the other
- Non-ohmic devices: Light dependent resistor, photoresistor; diodes

## Magnetism

### Magnets I

- Magnetic field strength $\propto \frac{1}{r^3}$

$$
\vec{F} = q\vec{v}\times \vec{B}, [N/C\cdot m/s]=[N/A\cdot m]=[T]
$$

$$
F=qvB\sin\theta
$$

- Magnetic field is defined by "Lorentz Force" on a charged particle moving in the field ("Tesla")

  - $1 G = 100 \mu T$, one Gauss

- No magnetic monopoles

- Motion of charged particles in a field
  $$
  qvB = \frac{mv^2}{r} \rightarrow r=\frac{mv}{qB}
  $$

  $$
  T=\frac{2\pi r}{v}=\frac{2 \pi m}{qB}
  $$

  - The period for the particle to go around is the same
  - Bubble chamber: liquid; Cloud chamber: vapour

- Solar wind $\rightarrow$ Aurora Borealis

- Hall effect: Magnetic field bends the charges in the current generating a voltage

- Mass Spectrometry
  $$
  F_{electric} = qE
  $$

  $$
  F_{magnetic}=qvB
  $$

  $$
  F_{electric} + F_{magnetic}=0
  $$

  $$
  R = \frac{mv}{qB}
  $$

- Carbon-14 Dating
  $$
  n + ^{14}_{7}N \rightarrow ^{14}_{6}C + p
  $$

  - $\beta$ decay - ($\tau \approx 8267$ yrs, $t_{\frac{1}{2}} \approx 5730$ yrs)

  $$
  ^{14}_{6}C \rightarrow ^{14}_{7}N + e^- + \bar{\nu_e}
  $$

### Magnets II

- Half-life ($\lambda$: chance of nucleus decaying per second, $N$: number of nuclei)
  $$
  \dv{N}{t} = -\lambda N
  $$

  $$
  t_{\frac{1}{2}}=\ln(2)\tau
  $$

- Cyclotron

  - Isochronous - constant orbit speed
    $$
    v=\frac{qrB}{m}
    $$

- Currents make magnetic fields - Clockwise if the current is pointing towards you
- Ampere's Law

$$
\oint \vec{B} \cdot \dd{\vec{L}}=\mu_0I
$$

$$
B = \frac{\mu_0 I}{2\pi r}
$$

- Solenoids ($N$ is the number of coils)

  - Inside the solenoid, all magnetic fields add up

  - Outside the solenoid, the fields cancel

  - More coils per unit length, greater magnetic field inside

  - Uniform in the inside
    $$
    B= \mu_0 nI, n=\frac{N}{L}
    $$

- Faraday's Law - Magnetic Flux ($Wb = T\cdot m^2$)

$$
\Phi_m = \int_s \vec{B} \cdot \hat{n}\dd A
$$

- Electric charges produce electric fields
- Electric fields induce charges
- Currents make magnetic fields
- **Change** in magnetic field induces current

### Magnetic Induction and LCR

- Mutual Inductance

- Lenz's Law

  - The direction of the induced *emf* drives current around a wire loop to always **oppose** the change in magnetic flux that causes the *emf*
    $$
    emf = \epsilon=-\dv{t} \int_s \vec{B} \cdot \hat{n}\dd A = -\dv{\Phi_m}{t}
    $$

- Iron core solenoids and Transformers

- Inducing a current: A conducting rod is pushed to "cut" the magnetic field lines to induce a current in the circuit

- Self-inductance

  - A field generated by a current can in turn affect that current, if current changes.

  - Inductance ($L$: $[V\cdot s/A] = [H]$, Henrys): Constant of proportionality between flux and current
    $$
    N\Phi_m = LI
    $$

    $$
    \epsilon = -L\dv{I}{t}=-N \dv{\Phi_m}{t}
    $$

  - Cylindrical Solenoid
    $$
    L_{solenoid} = \frac{N\Phi_m}{I} = \frac{\mu_0 N^2 A}{L}
    $$

- Energy in an Inductor
  $$
  P = \epsilon i = L\dv{i}{t}i
  $$

  $$
  U = \int_0^t P\dd t' = \frac{1}{2}LI^2
  $$

  - $R$: Viscous fluid
  - $C$: Spring
  - $L$: Mass

- Electronic Oscillator

## Nucleosynthesis

- Subatomic level - Forces are mediated by the exchange of virtual particles ($\gamma$: photon; $g$: gluon; $Z$: weak force; $W$: weak force)
  - Electromagnetic force: photons
  - Strong force: gluons (bind quarks into nucleons and nucleons into the nucleus)
  - Weak force: $W^{\pm}, Z^0$ - controls $\beta$ decay
- $\beta$ decay - (Flavour conservation, extra energy as kinetic energy)

$$
n^0 \rightarrow p^+ + e^- + \bar{\nu_e}
$$

$$
p^+ + n^0 \rightarrow ^2_1D + \gamma
$$

- Immediately after Big Bang...

  - The # of protons $\approx$ The # of neutrons ($t_{\frac{1}{2}}(n^0) \approx 14$ min $40$ sec)
  - Neutron has a chance to fuse with a proton to create a deuteron ($^2H$), most of which fuse further to form ($^4He$)
  - Potential well inside nuclei is deep enough for neutrons to be stable
  - An hour after, all $H$ and $He$ are formed, up to $^7Li$

- $amu = \frac{1}{12}m_{^{12}C} = 6p^+ + 6n^0 + 6e^-$

- Short range attraction from the strong force balancing long range repulsion by the electrostatic

- In Stars

  - Proton-Proton Fusion

    - Long tail to Maxwell-Boltzmann distribution
    - Large quantities of protons
    - Tunneling through the "Coulomb barrier"
    - More opportunities of fusing
    - More time for fusing

  - In smallish stars
    $$
    4^1H^+ + 2e^- \to ^4He^{2+} + 2\nu_e + 26.7MeV
    $$

    - Rate limiting step

    $$
    p + p \to ^2_1D + e^+ + \nu_e
    $$

    - 2.2% of the energy released goes to neutrinos, which have an average energy of $200keV$

- Stability of $^4He$

  - 2 protons + 2 neutrons
  - 2 spin up + 2 spin down (spins, like magnets, stick together if opposed)
  - Electrostatic repulsion overcome by attractive, short-range strong nuclear force
  - Very strongly bound for a light nucleus (bind energy: $28.3MeV$, $7.1MeV$ per nucleon)

- In Giants and Supergiants

  - Stellar cores hotter and denser
  - "Helium-burning"
  - Temperature high enough to overcome increasing Coulomb barrier of heavier nuclei
  - Heavier nuclei require some conversion of proton to neutrons to stay stable ($^{56}Fe$ is at the peak of the binding energy curve)

- Repulsive protons: short-range strong nuclear force starts to peter out

  - Limit on heavy stable nuclei at Lead and Bismuth
  - $^{232}Th$ and $^{238}U$ are unstable, but long mean life

- $^8Be$ is not stable

  - Three $^4He$ nuclei would have to interact at the same time and this would require a $^{12}C$ excited state at $7.68MeV$ to allow this - "Triple-$\alpha$" process
  - Energy accessible to the cores of red giants ($200MK$)

- Get past $^{56}Fe$

  - Supernova
    - $e^- + p^+ \to n + \nu_e$
    - The remnant after the explosion of supernova was a solar mass worth of $^{56}Ni$
    - When star runs out of fuel, gravity no longer balanced by the force of photons fighting their way to the surface
    - Supernova collapse so fast and so dense that the nuclei bigger than Fe-56 can be slammed together faster than it decays
    - Subsequent explosions disperses all the elements created into the galactic environment

- Conclusion

  - Universe old enough to complete one round of stellar evolution to provide the whole range of elements, and several gigayears into the next round for planetary formation and evolution of life
  - Extraordinary fine tolerances of the basic forces

## Constants and Useful Unit Conversions

Planck Constant
$$
h=6.626 \times 10^{-34}J\cdot s
$$
Electron Volts to Joules
$$
1eV=1.602 \times 10^{-19}J
$$
Boltzmann Constant
$$
k_B=1.380649 \times 10^{-23} m^2 \cdot kg \cdot s^{-2} \cdot K^{-1}
$$
Charge of an electron
$$
e=1.602 \times 10^{-19} C
$$
Coulomb Law's Constants
$$
k = \frac{1}{4\pi \epsilon_0} = 9 \times 10^9 N \cdot m^2 / C^2, \epsilon_0 \approx 8.85 \times 10^{-12} F/m
$$
Vacuum Permeability Constant
$$
\mu_0 = 1.256637062 \times 10^{-6} N/A^2
$$
