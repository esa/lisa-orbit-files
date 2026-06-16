### OEM Files in the TCB Time Scale

The following Orbit Ephemeris Message (OEM) files contain spacecraft state vectors expressed in the TCB (Barycentric Coordinate Time) time scale. They differ only in the sampling strategy applied to the underlying numerical integration.

The following gravitational bodies are included in the force model:

- **Earth**
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

- **Relative tolerance**: 1e-9
- **Absolute tolerance**: 1e-9

---
#### `*_lisa[1|2|3].oem`
Default LISA orbit files with an effective sampling interval of approximately **3 days**.  
These files are generated using:
- a numerical integration performed on a coarser internal time grid, and  
- **4× oversampling** using a dense Runge–Kutta interpolator to provide intermediate states.

---
#### `*_lisa[1|2|3]_no_ovrs.oem`
Orbit files **without oversampling**.  
The ephemeris points correspond **exactly to the integration grid** used by the numerical propagator.  
No intermediate points are generated.

---

#### `*_lisa[1|2|3]_step_1hour.oem`
Orbit files generated through **dense Runge–Kutta interpolation** on a **uniform 1‑hour output time step**.  
The propagation itself may still use adaptive internal step sizes; only the output cadence is fixed.