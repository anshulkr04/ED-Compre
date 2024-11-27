# Metal-Semiconductor Junction Fundamentals

## Table of Contents
1. [Energy Band Parameters](#energy-band-parameters)
2. [Junction Properties](#junction-properties)
3. [Schottky Barrier](#schottky-barrier)
4. [Depletion Region](#depletion-region)
5. [Ohmic vs Rectifying Contacts](#ohmic-vs-rectifying-contacts)

## Energy Band Parameters
### Metal Work Function
$$q\phi_m = E_0 - E_{fm}$$

### Semiconductor Electron Affinity
$$q\chi = E_0 - E_c$$

### Semiconductor Work Function
For n-type:
$$q\phi_s = q\chi + \frac{E_g}{2} - kT\ln(\frac{N_d}{n_i})$$

For p-type:
$$q\phi_s = q\chi + \frac{E_g}{2} + kT\ln(\frac{N_a}{n_i})$$

## Junction Properties
### Built-in Potential
For n-type:
$$qV_0 = q(\phi_m - \phi_s) = q\phi_m - (q\chi + \frac{E_g}{2} - kT\ln(\frac{N_d}{n_i}))$$

For p-type:
$$qV_0 = q(\phi_s - \phi_m) = [q\chi + \frac{E_g}{2} + kT\ln(\frac{N_a}{n_i})] - q\phi_m$$

### Barrier Height
For n-type:
$$q\phi_B = q(\phi_m - \chi)$$

For p-type:
$$q\phi_B = (E_0 - E_v) - q\phi_m = q\chi + E_g - q\phi_m$$

## Depletion Region
### Depletion Width
$$W = \sqrt{\frac{2\epsilon V_0}{qN_d}}$$ (for n-type)
$$W = \sqrt{\frac{2\epsilon V_0}{qN_a}}$$ (for p-type)

### Electric Field
Maximum electric field:
$$E_{max} = \frac{q}{\epsilon}N_dW$$ (for n-type)
$$E_{max} = \frac{q}{\epsilon}N_aW$$ (for p-type)

## Ohmic vs Rectifying Contacts
### Conditions for Ohmic Contact
For n-type: $$\phi_m < \phi_s$$
For p-type: $$\phi_m > \phi_s$$

### Conditions for Rectifying Contact (Schottky)
For n-type: $$\phi_m > \phi_s$$
For p-type: $$\phi_m < \phi_s$$

## Important Parameters
- $$E_0$$ = Vacuum energy level
- $$E_c$$ = Conduction band energy
- $$E_v$$ = Valence band energy
- $$E_f$$ = Fermi level
- $$E_g$$ = Band gap
- $$\phi_m$$ = Metal work function
- $$\phi_s$$ = Semiconductor work function
- $$\chi$$ = Electron affinity
