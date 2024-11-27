# MOS Capacitor Fundamentals

## Table of Contents
1. [Operating Regions](#operating-regions)
2. [Threshold Voltage](#threshold-voltage)
3. [Capacitance](#capacitance)
4. [Surface Potential](#surface-potential)
5. [Charge Relations](#charge-relations)

## Operating Regions
1. Accumulation ($$V_G < 0$$ for p-type)
2. Depletion ($$0 < V_G < V_{TH}$$)
3. Inversion ($$V_G > V_{TH}$$)

## Threshold Voltage
### Ideal MOS
$$V_{TH} = 2\phi_F + \frac{Q_d}{C_{ox}}$$

where $$\phi_F = V_T\ln(\frac{N_a}{n_i})$$

### Non-ideal MOS
$$V_{TH} = \phi_{ms} - \frac{Q_I}{C_{ox}} - \frac{Q_d}{C_{ox}} + 2\phi_F$$

### Metal-Semiconductor Work Function
For n+ poly gate on p-substrate:
$$\phi_{ms} = -[\frac{E_g}{2q} + V_T\ln(\frac{N_a}{n_i})]$$

## Capacitance
### Oxide Capacitance
$$C_{ox} = \frac{\epsilon_{ox}}{t_{ox}}$$

### Depletion Capacitance
$$C_d = \frac{\epsilon_s}{W}$$

### Total Capacitance
$$\frac{1}{C_T} = \frac{1}{C_{ox}} + \frac{1}{C_d}$$

## Surface Potential
### General Expression
$$q\phi_s = kT\ln(\frac{n_s}{n_i}) + kT\ln(\frac{N_a}{n_i})$$

### Strong Inversion
$$\phi_s = 2\phi_F = 2V_T\ln(\frac{N_a}{n_i})$$

## Depletion Width
$$W = \sqrt{\frac{2\epsilon_s\phi_s}{qN_a}}$$

Maximum depletion width:
$$W_m = 2\sqrt{\frac{\epsilon_sV_T\ln(\frac{N_a}{n_i})}{qN_a}}$$

## Charge Relations
### Inversion Charge
$$Q_i = -C_{ox}(V_G - V_{TH})$$

### Depletion Charge
$$Q_d = -qN_aW$$

## Important Parameters
- $$\epsilon_{ox}$$ = Oxide permittivity
- $$\epsilon_s$$ = Semiconductor permittivity
- $$t_{ox}$$ = Oxide thickness
- $$N_a$$ = Substrate doping
- $$n_i$$ = Intrinsic carrier concentration
- $$\phi_{ms}$$ = Metal-semiconductor work function difference
- $$Q_I$$ = Interface charge
- $$V_T$$ = Thermal voltage (kT/q)
