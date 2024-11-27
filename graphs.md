# Semiconductor Device Physics

## Table of Contents
1. [PN Junction](#pn-junction)
2. [Metal-Semiconductor Junction](#metal-semiconductor-junction)
3. [Junction Field Effect Transistor](#jfet)
4. [MOS Capacitor](#mos-capacitor)

# PN Junction

## Table of Contents
1. [Basic Concepts](#basic-concepts)
2. [Built-in Potential](#built-in-potential)
3. [Depletion Region](#depletion-region)
4. [Electric Field](#electric-field)
5. [Junction Capacitance](#junction-capacitance)
6. [Current Equations](#current-equations)

## Key Characteristics

### I-V Characteristic
```mermaid
graph TB
    subgraph I-V Curve
    style I-V Curve fill:#f9f9f9,stroke:#333,stroke-width:2px
    A[Forward Bias] -->|Exponential increase| B[Current flow]
    C[Reverse Bias] -->|Very small current| D[Saturation current]
    D -->|Breakdown| E[Avalanche]
    end
```

### Energy Band Diagram
```mermaid
graph LR
    subgraph Band Diagram
    style Band Diagram fill:#f9f9f9,stroke:#333,stroke-width:2px
    A[P-type] -->|Band bending| B[Junction]
    B -->|Band bending| C[N-type]
    end
```

[Rest of PN Junction content as before...]

# Metal-Semiconductor Junction

### Band Diagram
```mermaid
graph LR
    subgraph Energy Bands
    style Energy Bands fill:#f9f9f9,stroke:#333,stroke-width:2px
    A[Metal] -->|Barrier| B[Semiconductor]
    end
```

[Rest of Metal-Semiconductor content as before...]

# JFET

### Characteristics
```mermaid
graph TB
    subgraph I-V Characteristics
    style I-V Characteristics fill:#f9f9f9,stroke:#333,stroke-width:2px
    A[Linear Region] -->|Pinch-off| B[Saturation Region]
    end
```

[Rest of JFET content as before...]

# MOS Capacitor

### C-V Characteristic
```mermaid
graph TB
    subgraph C-V Curve
    style C-V Curve fill:#f9f9f9,stroke:#333,stroke-width:2px
    A[Accumulation] -->|Depletion| B[Inversion]
    end
```

[Rest of MOS Capacitor content as before...]

## Notes on Diagrams:
- The diagrams are implemented using Mermaid graph syntax
- Each section includes relevant visual representations of key concepts
- Diagrams are integrated with the theoretical content for better understanding
- Interactive elements are preserved in the markdown format
