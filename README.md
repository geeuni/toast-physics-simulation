# 🍞 Tumbling Toast Simulation

A browser-based physics simulation based on Bacon, Heald & James, *Am. J. Phys.* 69, 38–43 (2001).  
No installation required — just open `tumbling_toast_simulation.html` in any browser.

---

## Physics

The simulation models three phases of toast falling off a table:

1. **No-slip rotation** — toast pivots about the table edge (Eq. 13)
2. **Slip phase** — kinetic friction takes over once Ff/FN reaches μₛ (Eq. 4, 5, 7)
3. **Free fall** — rotation continues until the toast hits the floor

> Key insight: slipping must be included to match real angular velocities. No-slip theory alone underestimates ω significantly.

**Landing rule:** butter-side down if 90° < α_T < 270°

---

## Parameters

| Symbol | Description | Default |
|--------|-------------|---------|
| d₀ | Initial overhang | 1.10 cm |
| μₛ | Static friction coefficient | 0.32 |
| μₖ | Kinetic friction coefficient | 0.24 |
| H | Table height | 76 cm |
| a | Toast half-length | 5.1 cm |
| b | Toast thickness | 1.3 cm |

---

## Project Context

BS103 General Physics I course project — DGIST, Spring 2026.

---

## Reference

M. E. Bacon, G. Heald, and M. James, "A closer look at tumbling toast," *Am. J. Phys.* **69**, 38 (2001). https://doi.org/10.1119/1.1289213
