# Junction Field Effect Transistor (JFET) Fundamentals

## Table of Contents
1. [Basic Structure](#basic-structure)
2. [Channel Properties](#channel-properties)
3. [Operating Regions](#operating-regions)
4. [Current Equations](#current-equations)
5. [Key Parameters](#key-parameters)

## Basic Structure
The JFET is a three-terminal device with:
- Source (S)
- Drain (D)
- Gate (G)

## Channel Properties
### Channel Width
$$a = W(x) + h(x)$$
where:
- a = Metallurgical half-width
- W(x) = Depletion half-width
- h(x) = Channel half-width

### Depletion Width
$$W(x) = \sqrt{\frac{2\epsilon(V_0 + V(x))}{qN_d}}$$ (for n-channel)

## Operating Regions
### Pinch-off Voltage
$$V_P = \frac{qa^2N_d}{2\epsilon} - V_0$$

### Linear Region Current
$$I_D = G_0V_P[\frac{V_D}{V_P} + \frac{2}{3}(-\frac{V_G}{V_P})^{3/2} - \frac{2}{3}(\frac{V_D - V_G}{V_P})]$$

where $$G_0 = \frac{2aZ\sigma}{L}$$

### Saturation Region Current
$$I_D(sat) = G_0V_P[\frac{V_G}{V_P} + \frac{2}{3}(-\frac{V_G}{V_P})^{3/2} + \frac{1}{3}]$$

Simplified form:
$$I_D = I_{DSS}(1 + \frac{V_G}{V_P})^2$$

### Transconductance
$$g_m = \frac{\partial I_D}{\partial V_D} = G_0[1 - (-\frac{V_G}{V_P})^{1/2}]$$

## Channel Current
Cross-sectional area:
$$A(x) = 2Zh(x)$$

Current density:
$$I_D = A(x)\sigma\frac{dV(x)}{dx}$$

## Key Parameters
- Z = Channel depth
- L = Channel length
- σ = Channel conductivity
- $$I_{DSS}$$ = Drain saturation current at $$V_G = 0$$
- $$V_P$$ = Pinch-off voltage

## Operating Conditions
1. Linear Region: $$V_D < V_P$$
2. Saturation Region: $$V_D \geq V_P$$
3. Pinch-off: $$V_D = V_P$$
