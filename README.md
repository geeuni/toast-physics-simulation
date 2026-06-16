# 🍞 Tumbling Toast Simulation

Physics simulation based on **Bacon, Heald & James (2001)**  
*"A closer look at tumbling toast"* — Am. J. Phys. 69, 38–43  
[https://doi.org/10.1119/1.1289213](https://doi.org/10.1119/1.1289213)

---

## Demo

Open `tumbling_toast_simulation.html` in any browser — no installation required.

---

## Physics Overview

The simulation implements the three-phase model from the paper:

| Phase | Description | Key Equation |
|-------|-------------|--------------|
| **Phase 1** | No-slip rotation about table edge | Eq. (13): θ̈ = r₀g·cos(θ−β₀) / ((a²+b²)/3 + d₀²) |
| **Phase 2** | Slip phase with kinetic friction | Eq. (4)(5)(7): full coupled ODE system |
| **Phase 3** | Free fall & landing prediction | y(t) = y₀ + ẏ₀t − 4.9t² − a\|sin(α₀ + α̇₀t)\| |

**Key finding:** Slipping *must* be included to match experimental angular velocities (Fig. 7 of paper). Simple no-slip theory significantly underestimates ω.

**Butter-side down condition:** 90° < α_T < 270°

---

## Features

- 🎬 Animated 3-phase toast tumbling visualization
- 📊 Real-time angular velocity graph (ω vs time)
- 📈 Overhang sweep graph reproducing Fig. 8 of the paper
- 🎛️ Adjustable parameters: d₀, μₛ, μₖ, table height H, toast dimensions

---

## Parameters

| Symbol | Description | Default (paper value) |
|--------|-------------|----------------------|
| d₀ | Initial overhang | 1.10 cm |
| μₛ | Static friction coefficient | 0.32 |
| μₖ | Kinetic friction coefficient | 0.24 |
| H | Table height | 76 cm |
| a | Toast half-length | 5.1 cm (2a = 10.2 cm) |
| b | Toast thickness | 1.3 cm |

---

## Project Context

Created as part of the **BS103 General Physics I** course project at DGIST (2026 Spring).  
Paper selected from the *American Journal of Physics* per course requirements.

---

## Reference

M. E. Bacon, G. Heald, and M. James,  
"A closer look at tumbling toast,"  
*Am. J. Phys.* **69**, 38–43 (2001).  
https://doi.org/10.1119/1.1289213
