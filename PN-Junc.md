# PN Junction Fundamentals

## Table of Contents
1. [Basic Concepts](#basic-concepts)
2. [Built-in Potential](#built-in-potential)
3. [Depletion Region](#depletion-region)
4. [Electric Field](#electric-field)
5. [Junction Capacitance](#junction-capacitance)
6. [Current Equations](#current-equations)

## Basic Concepts
A PN junction is formed when P-type and N-type semiconductors are brought together. The junction creates a depletion region due to the diffusion of charge carriers.

## Built-in Potential
The built-in potential (V₀) across the junction at equilibrium:

$$V_0 = V_T \ln(\frac{N_aN_d}{n_i^2})$$

where:
- $$V_T$$ = Thermal voltage (kT/q)
- $$N_a$$ = Acceptor concentration
- $$N_d$$ = Donor concentration
- $$n_i$$ = Intrinsic carrier concentration

## Depletion Region
The depletion width (W) is given by:

$$W = \sqrt{\frac{2\epsilon(V_0 + V)}{q}(\frac{1}{N_a} + \frac{1}{N_d})}$$

For P+N junction (Na >> Nd):
$$W \approx \sqrt{\frac{2\epsilon(V_0 + V)}{qN_d}}$$

Depletion region charge balance:
$$N_ax_p = N_dx_n$$

where:
- $$x_p$$ = Depletion width in P-region
- $$x_n$$ = Depletion width in N-region

## Electric Field
Maximum electric field at the junction:

$$E_0 = \frac{qN_aN_d}{(N_a + N_d)\epsilon}W$$

Electric field distribution:
- P-side: $$E(x) = -\frac{qN_a(x + x_p)}{\epsilon}$$ for $$-x_p < x < 0$$
- N-side: $$E(x) = \frac{qN_d(x - x_n)}{\epsilon}$$ for $$0 < x < x_n$$

## Junction Capacitance
Junction (depletion) capacitance per unit area:

$$C_j = \sqrt{\frac{q\epsilon}{2(V_0 + V)}(\frac{N_aN_d}{N_a + N_d})}$$

For reverse bias:
$$\frac{1}{C_j^2} = \frac{2(V_0 + V)}{q\epsilon}(\frac{1}{N_a} + \frac{1}{N_d})$$

## Current Equations
Diode current equation:

$$I = I_s(e^{V/V_T} - 1)$$

where saturation current $$I_s$$ is:

$$I_s = qA(\frac{D_p}{L_p}p_n + \frac{D_n}{L_n}n_p)$$

Diffusion lengths:
- Holes: $$L_p = \sqrt{D_p\tau_p}$$
- Electrons: $$L_n = \sqrt{D_n\tau_n}$$

### Important Parameters:
- $$\epsilon$$ = Semiconductor permittivity
- $$q$$ = Electronic charge
- $$D_p, D_n$$ = Diffusion coefficients
- $$\tau_p, \tau_n$$ = Carrier lifetimes
- $$A$$ = Junction area

## Additional Notes
1. Forward bias reduces the potential barrier
2. Reverse bias increases the depletion width
3. Temperature affects built-in potential and current
4. Breakdown occurs at high reverse bias due to:
   - Avalanche multiplication
   - Zener effect
