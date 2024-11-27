# Thermal Equilibrium in Semiconductors
*Complete Theory and Analysis*

## Table of Contents
1. [Basic Concepts](#basic-concepts)
2. [Carrier Concentrations](#carrier-concentrations)
3. [Intrinsic Semiconductors](#intrinsic-semiconductors)
4. [Extrinsic Semiconductors](#extrinsic-semiconductors)
5. [Fermi Level Analysis](#fermi-level-analysis)
6. [Temperature Effects](#temperature-effects)
7. [Compensated Semiconductors](#compensated-semiconductors)

## Basic Concepts

### Definition
Thermal Equilibrium: State where energy remains spatially and temporally constant. For every process, there exists an inverse process conserving total energy.

### Occupied and Vacant States
Number of occupied states:
$$n = \int_{E_1}^{E_2} g(E)f(E)dE$$

Number of vacant states:
$$p = \int_{E_1}^{E_2} g(E)(1-f(E))dE$$

### Density of States
Conduction band:
$$g_c(E) = \frac{4π(2m_n^*)^{3/2}}{h^3}\sqrt{E-E_c}$$

Valence band:
$$g_v(E) = \frac{4π(2m_p^*)^{3/2}}{h^3}\sqrt{E_v-E}$$

## Carrier Concentrations

### Electron Concentration
$$n_0 = N_c\exp(-\frac{E_c-E_f}{kT})$$

where effective density of states:
$$N_c = 2(\frac{2πm_n^*kT}{h^2})^{3/2}$$

### Hole Concentration
$$p_0 = N_v\exp(-\frac{E_f-E_v}{kT})$$

where:
$$N_v = 2(\frac{2πm_p^*kT}{h^2})^{3/2}$$

## Intrinsic Semiconductors

### Intrinsic Carrier Concentration
$$n_i = \sqrt{N_cN_v}e^{-E_g/2kT}$$

Temperature dependence:
$$n_i(T) = 2(\frac{2πkT}{h^2})^{3/2}(m_n^*m_p^*)^{3/4}e^{-E_g/2kT}$$

### Intrinsic Fermi Level
$$E_i = \frac{E_c + E_v}{2} + \frac{3}{4}\ln(\frac{m_p^*}{m_n^*})$$

For silicon:
$$E_i = \frac{E_c + E_v}{2} - 12.8\text{ meV}$$

## Extrinsic Semiconductors

### N-type Semiconductor
Electron concentration:
$$n_0 = n_i\exp(\frac{E_f-E_i}{kT})$$

Hole concentration:
$$p_0 = n_i\exp(\frac{E_i-E_f}{kT})$$

Under complete ionization:
$$n_0 ≈ N_d$$ and $$p_0 = \frac{n_i^2}{N_d}$$

### P-type Semiconductor
Complete ionization:
$$p_0 ≈ N_a$$ and $$n_0 = \frac{n_i^2}{N_a}$$

### Mass Action Law
Valid for all cases:
$$n_0p_0 = n_i^2$$

## Fermi Level Analysis

### N-type Semiconductor
$$E_c - E_f = kT\ln(\frac{N_c}{n_0})$$

### P-type Semiconductor
$$E_f - E_v = kT\ln(\frac{N_v}{p_0})$$

### Temperature Effects
$$E_f - E_i = kT\ln(\frac{n_0}{n_i})$$ (n-type)
$$E_i - E_f = kT\ln(\frac{p_0}{n_i})$$ (p-type)

## Temperature Effects

### Carrier Concentration vs Temperature
$$n_i(T_2) = n_i(T_1)(\frac{T_2}{T_1})^{3/2}e^{E_g/2k(1/T_1 - 1/T_2)}$$

### Three Temperature Regions
1. Partial Ionization (Low T)
   - $$n_0(T) = N_d^+$$ where $$N_d^+ < N_d$$

2. Extrinsic Region (Medium T)
   - $$n_0 ≈ N_d$$ and $$p_0 = \frac{n_i^2}{N_d}$$

3. Intrinsic Region (High T)
   - $$n_0 ≈ p_0 ≈ n_i(T)$$

## Compensated Semiconductors

### Charge Neutrality
$$n_0 + N_a^- = p_0 + N_d^+$$

### N-type ($$N_d > N_a$$)
$$n_0 = \frac{N_d-N_a}{2} + \sqrt{(\frac{N_d-N_a}{2})^2 + n_i^2}$$
$$p_0 = \frac{n_i^2}{n_0}$$

### P-type ($$N_a > N_d$$)
$$p_0 = \frac{N_a-N_d}{2} + \sqrt{(\frac{N_a-N_d}{2})^2 + n_i^2}$$
$$n_0 = \frac{n_i^2}{p_0}$$

### Special Case: $$N_a = N_d$$
$$n_0 = p_0 = n_i$$

## Important Problem-Solving Tips

1. **Temperature Analysis**
   - Always check operating temperature region
   - Consider temperature effects on $$n_i$$
   - Account for partial ionization at low T

2. **Doping Effects**
   - Check if $$N_d$$ or $$N_a >> n_i$$
   - Verify complete ionization assumption
   - Consider compensation effects

3. **Fermi Level Calculations**
   - Use appropriate reference ($$E_c$$, $$E_v$$, or $$E_i$$)
   - Account for temperature dependence
   - Consider degenerate cases for heavy doping
