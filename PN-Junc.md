# Complete PN Junction Theory and Formulas

## Table of Contents
1. [Built-in Potential and Equilibrium](#built-in-potential-and-equilibrium)
2. [Depletion Region](#depletion-region)
3. [Electric Field](#electric-field)
4. [One-Sided Junctions](#one-sided-junctions)
5. [Junction Capacitance](#junction-capacitance)
6. [Current Equations](#current-equations)
7. [Carrier Distribution](#carrier-distribution)
8. [Diffusion and Continuity](#diffusion-and-continuity)

## Built-in Potential and Equilibrium

### Basic Built-in Potential
$$V_0 = V_T \ln(\frac{N_aN_d}{n_i^2})$$

### Carrier Concentrations
At equilibrium:
$$p(−x_p) = p_p$$ and $$p(x_n) = p_n$$

Under equilibrium conditions:
$$\frac{p(-x_p)}{p(x_n)} = e^{V_0/V_T} \implies \frac{p_p}{p_n} = e^{V_0/V_T}$$

In extrinsic regions:
$$p_p = N_a$$
$$n_n = N_d$$
$$n_p = \frac{n_i^2}{N_a}$$
$$p_n = \frac{n_i^2}{N_d}$$

## Depletion Region

### Width Calculations
Total depletion width:
$$W = x_p + x_n$$

Individual depletion widths:
$$x_p = \frac{N_d}{N_a + N_d}W$$
$$x_n = \frac{N_a}{N_a + N_d}W$$

Charge balance:
$$qAN_ax_p = qAN_dx_n$$

### Width Under Bias
$$W = \sqrt{\frac{2\epsilon(V_0 + V)}{q}(\frac{1}{N_a} + \frac{1}{N_d})}$$

## Electric Field

### Field Distribution
P-side:
$$E(x) = -\frac{qN_a(x + x_p)}{\epsilon}$$ for $$-x_p < x < 0$$

N-side:
$$E(x) = \frac{qN_d(x - x_n)}{\epsilon}$$ for $$0 < x < x_n$$

### Maximum Electric Field
$$E_0 = \frac{qN_ax_p}{\epsilon} = \frac{qN_dx_n}{\epsilon}$$
$$E_0 = \frac{q}{\epsilon}\frac{N_aN_d}{N_a + N_d}W$$

## One-Sided Junctions

### P+N Junction ($$N_a >> N_d$$)
Depletion width:
$$x_n \approx W = \sqrt{\frac{2\epsilon V_0}{qN_d}}$$

Electric field:
$$E_{max} = \frac{q}{\epsilon}N_dW$$

Built-in potential:
$$V_0 = \frac{q}{2\epsilon}N_dW^2$$

### PN+ Junction ($$N_d >> N_a$$)
Similar equations with $$N_a$$ and $$N_d$$ swapped

## Junction Capacitance

### Depletion Capacitance
$$C_j = \sqrt{\frac{q\epsilon}{2(V_0 + V)}(\frac{N_aN_d}{N_a + N_d})}$$

### Capacitance-Voltage Relationship
$$\frac{1}{C_j^2} = \frac{2(V_0 + V)}{q\epsilon}(\frac{1}{N_a} + \frac{1}{N_d})$$

For one-sided junctions:
$$C_j = \sqrt{\frac{q\epsilon N_d}{2(V_0 + V)}}$$ (P+N junction)
$$C_j = \sqrt{\frac{q\epsilon N_a}{2(V_0 + V)}}$$ (PN+ junction)

## Current Equations

### Diode Equation
$$I = I_s(e^{V/V_T} - 1)$$

### Saturation Current
$$I_s = qA(\frac{D_p}{L_p}p_n + \frac{D_n}{L_n}n_p)$$

### Under Forward Bias
Excess carrier concentrations:
$$\Delta p_n = p_n(e^{V/V_T} - 1)$$
$$\Delta n_p = n_p(e^{V/V_T} - 1)$$

## Carrier Distribution

### Minority Carrier Distribution
In n-region:
$$\delta p(x) = \Delta p_n e^{-x/L_p}$$

In p-region:
$$\delta n(x) = \Delta n_p e^{-x/L_n}$$

### Diffusion Lengths
$$L_p = \sqrt{D_p\tau_p}$$
$$L_n = \sqrt{D_n\tau_n}$$

## Diffusion and Continuity

### Continuity Equations
Without electric field:
$$\frac{\partial \delta p}{\partial t} = D_p\frac{\partial^2\delta p}{\partial x^2} - \frac{\delta p}{\tau_p}$$
$$\frac{\partial \delta n}{\partial t} = D_n\frac{\partial^2\delta n}{\partial x^2} - \frac{\delta n}{\tau_n}$$

With constant electric field:
$$\frac{\partial \delta p}{\partial t} = D_p\frac{\partial^2\delta p}{\partial x^2} - \mu_pE\frac{\partial \delta p}{\partial x} + g_p - \frac{\delta p}{\tau_p}$$
$$\frac{\partial \delta n}{\partial t} = D_n\frac{\partial^2\delta n}{\partial x^2} + \mu_nE\frac{\partial \delta n}{\partial x} + g_n - \frac{\delta n}{\tau_n}$$

### Current Components
Hole current:
$$J_p(x) = q\mu_pp(x)E(x) - qD_p\frac{\partial \delta p}{\partial x}$$

Electron current:
$$J_n(x) = q\mu_nn(x)E(x) + qD_n\frac{\partial \delta n}{\partial x}$$

### Steady State Solutions
General solution for holes:
$$\delta p(x) = C_1e^{-x/L_p} + C_2e^{x/L_p}$$

General solution for electrons:
$$\delta n(x) = C_1e^{-x/L_n} + C_2e^{x/L_n}$$

## Breakdown Mechanisms

### Avalanche Multiplication
$$M = \frac{1}{1-(V/V_{BR})^n}$$ where $$3 \leq n \leq 6$$
