### OEM Files in the TCB Time Scale

The following Orbit Ephemeris Message (OEM) files contain spacecraft state vectors expressed in the TCB (Barycentric Coordinate Time) time scale. They differ only in the sampling strategy applied to the underlying numerical integration.

The dynamical model follows **CReMA 2.0** in all aspects except for files containing the "nonsph" string. For these the Earth’s gravity field, which is represented using a **spherical-harmonic expansion up to degree and order 3 (3×3)** instead of the point‑mass model adopted in CReMA. The following gravitational bodies are included in the force model:

- **Earth** (3×3 gravity field for "nonsph" cases)
- **Sun**
- **Moon**
- **Mercury Barycenter**
- **Venus Barycenter**
- **Mars Barycenter**
- **Jupiter Barycenter**
- **Saturn Barycenter**
- **Uranus Barycenter**
- **Neptune Barycenter**
- **Deterministic spacecraft self‑gravity**, modeled as a linear acceleration variation between **−2 nm/s²** and **+2 nm/s²**

Integration tolerances:

- **Relative tolerance**: 1e-15
- **Absolute tolerance**: 1e-15
---

#### `*_nonsph_lisa[1|2|3]_no_ovrs.oem`
Orbit files **without oversampling**.  
The ephemeris points correspond **exactly to the integration grid** used by the numerical propagator.  
No intermediate points are generated.

---

#### `*_nonsph_lisa[1|2|3]_step_1hour.oem`
Orbit files generated through **dense Runge–Kutta interpolation** on a **uniform 1‑hour output time step**.  
The propagation itself may still use adaptive internal step sizes; only the output cadence is fixed.

---

#### `*_lisa[1|2|3]_step_1hour.oem`
Orbit files generated fixed **uniform 1-hour step size**