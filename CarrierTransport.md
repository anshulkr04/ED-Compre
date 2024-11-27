# Carrier Transport in Semiconductors
*Complete Theory and Analysis*

## Table of Contents
1. [Drift Mechanics](#drift-mechanics)
2. [Mobility](#mobility)
3. [Current Density](#current-density)
4. [Conductivity and Resistivity](#conductivity-and-resistivity)
5. [Diffusion](#diffusion)
6. [Einstein Relation](#einstein-relation)
7. [Energy Band Diagrams](#energy-band-diagrams)
8. [Hall Effect](#hall-effect)

## Drift Mechanics

### Force and Velocity Relationships
- Applied force: $$F = qE$$
- Peak velocity: $$v_{max} = \frac{qE}{m_p^*}τ_c$$
- Average drift velocity: $$v_d = \frac{qE}{m_p^*}τ_c = μE$$

### Mobility Definition
$$v_d = μE$$
- Holes: $$v_d = μ_pE$$
- Electrons: $$v_d = -μ_nE$$

## Mobility

### Temperature Dependencies
1. **Lattice Scattering**:
   $$μ_L \propto T^{-3/2}$$

2. **Ionized Impurity Scattering**:
   $$μ_I \propto \frac{T^{3/2}}{N_I}$$
   where $$N_I = N_d^+ + N_a^-$$

3. **Combined Mobility**:
   $$\frac{1}{μ} = \frac{1}{μ_I} + \frac{1}{μ_L}$$

## Current Density

### Basic Definitions
Volume charge density:
- Holes: $$ρ_p = qp$$
- Electrons: $$ρ_n = -qn$$

### Current Components
1. **Hole Current**:
   $$J_p = qpμ_pE$$

2. **Electron Current**:
   $$J_n = qnμ_nE$$

3. **Total Current**:
   $$J = J_p + J_n = q(pμ_p + nμ_n)E = σE$$

## Conductivity and Resistivity

### Conductivity
$$σ = q(pμ_p + nμ_n)$$

### Resistivity
$$ρ = \frac{1}{q(pμ_p + nμ_n)}$$

### Temperature Effects
1. **Intrinsic Semiconductor**:
   $$σ_i \propto e^{-E_g/2kT}$$
   $$ρ \propto e^{E_g/2kT}$$

2. **Extrinsic Semiconductor**:
   $$σ_i \propto T^{-3/2}$$
   $$ρ \propto T^{3/2}$$

## Diffusion

### Diffusion Current Density
$$J_n = qD_n\frac{dn}{dx}$$
$$J_p = -qD_p\frac{dp}{dx}$$

### Diffusion Coefficient
$$D = v_{th}λ$$
where:
- $$v_{th}$$ = Thermal velocity
- $$λ$$ = Mean free path

## Einstein Relation

### Basic Relationship
$$\frac{D}{μ} = \frac{D_p}{μ_p} = \frac{D_n}{μ_n} = \frac{kT}{q} = V_T$$

### Temperature Dependence
$$D \propto \frac{1}{\sqrt{T}}$$ (Intrinsic)
$$D \propto T^{5/2}$$ (Low T, Extrinsic)
$$D \propto \frac{1}{\sqrt{T}}$$ (High T, Extrinsic)

## Energy Band Diagrams

### Field and Potential Relationships
$$E_x = -\frac{dV}{dx}$$
$$E_c(x) = C - qV(x)$$

### Energy Band Variations
$$\frac{dE_c}{dx} = \frac{dE_v}{dx} = \frac{dE_i}{dx}$$

### Carrier Gradients
$$\frac{dE_i}{dx} = -\frac{kT}{n(x)}\frac{dn}{dx}$$
$$\frac{dE_i}{dx} = \frac{kT}{p(x)}\frac{dp}{dx}$$

## Hall Effect

### Hall Voltage
For p-type:
$$V_H = \frac{I_xB_z}{qdp}$$

For n-type:
$$V_H = -\frac{I_xB_z}{qdn}$$

### Carrier Concentration
$$p = \frac{I_xB_z}{qdV_H}$$ (p-type)
$$n = -\frac{I_xB_z}{qdV_H}$$ (n-type)

### Mobility
$$μ_p = \frac{I_xL}{qWdpV_0}$$ (p-type)
$$μ_n = \frac{I_xL}{qWdnV_0}$$ (n-type)

Now, let me create notes for Non-equilibrium Excess Carriers.


# Non-equilibrium Excess Carriers
*Complete Theory and Analysis*

## Table of Contents
1. [Generation and Recombination](#generation-and-recombination)
2. [Steady State Analysis](#steady-state-analysis)
3. [Recombination Lifetime](#recombination-lifetime)
4. [Continuity Equations](#continuity-equations)
5. [Diffusion Equations](#diffusion-equations)
6. [Quasi-Fermi Levels](#quasi-fermi-levels)

## Generation and Recombination

### Thermal Generation
- Generation rate: $$G_{p0} = G_{n0}$$
- Recombination rate: $$R = α_rn_0p_0$$
- At equilibrium: $$G_{p0} = G_{n0} = R_{p0} = R_{n0} = α_rn_i^2$$

### Excess Carriers
$$n(t) = n_0 + δn(t)$$
$$p(t) = p_0 + δp(t)$$

From charge neutrality:
$$δp(t) = δn(t)$$

## Steady State Analysis

### Generation-Recombination Balance
$$G = R = \frac{δn}{τ_n}$$

### Excess Carrier Concentrations
$$δn = δp = Gτ_n$$

For indirect recombination:
$$δn = Gτ_n$$
$$δp = Gτ_p$$

### Photo-Conductivity
$$σ = σ_0 + q(δnμ_n + δpμ_p)$$
$$Δσ = qG(τ_nμ_n + τ_pμ_p)$$

## Recombination Lifetime

### Basic Definition
$$τ_n = \frac{1}{α_r(n_0 + p_0)}$$

### Time Dependence
$$δn(t) = δn(0)e^{-t/τ_n}$$
$$δp(t) = δp(0)e^{-t/τ_p}$$

### Recombination Rate
$$R = -\frac{dδn(t)}{dt} = α_r(n_0 + p_0)δn(t) = \frac{δn(t)}{τ_n}$$

## Continuity Equations

### General Form
$$\frac{\partial p}{\partial t} = -\frac{1}{q}\frac{\partial J_p(x)}{\partial x} + G_p - \frac{p}{τ_p}$$
$$\frac{\partial n}{\partial t} = \frac{1}{q}\frac{\partial J_n(x)}{\partial x} + G_n - \frac{n}{τ_n}$$

### With Electric Field
$$\frac{\partial δp}{\partial t} = D_p\frac{\partial^2δp}{\partial x^2} - μ_pE\frac{\partial δp}{\partial x} + g_p - \frac{δp}{τ_p}$$
$$\frac{\partial δn}{\partial t} = D_n\frac{\partial^2δn}{\partial x^2} + μ_nE\frac{\partial δn}{\partial x} + g_n - \frac{δn}{τ_n}$$

## Diffusion Equations

### One-Dimensional Form
$$\frac{\partial^2(δp)}{\partial x^2} = \frac{δp}{L_p^2}$$
$$\frac{\partial^2(δn)}{\partial x^2} = \frac{δn}{L_n^2}$$

### Diffusion Length
$$L_p = \sqrt{D_pτ_p}$$
$$L_n = \sqrt{D_nτ_n}$$

### Solutions
General solution for holes:
$$δp(x) = C_1e^{-x/L_p} + C_2e^{x/L_p}$$

General solution for electrons:
$$δn(x) = C_1e^{-x/L_n} + C_2e^{x/L_n}$$

## Quasi-Fermi Levels

### Carrier Concentrations
$$n_0 + δn = n_ie^{(E_{Fn} - E_i)/kT}$$
$$p_0 + δp = n_ie^{(E_i - E_{Fp})/kT}$$

### Level Calculations
$$E_{Fn}-E_i = kT\ln(\frac{n_0 + δn}{n_i})$$
$$E_i-E_{Fp} = kT\ln(\frac{p_0 + δp}{n_i})$$

These notes include all formulas and concepts required for solving advanced problems in semiconductor physics. Would you like me to:
1. Add more example problems?
2. Expand on any particular section?
3. Include more practical applications?
4. Add visual representations of key concepts?
