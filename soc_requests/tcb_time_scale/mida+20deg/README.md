### OEM Files in the TCB Time Scale

The following Orbit Ephemeris Message (OEM) files contain spacecraft state vectors expressed in the TCB (Barycentric Coordinate Time) time scale. They differ only in the sampling strategy applied to the underlying numerical integration.

The dynamical model follows **CReMA 2.0** in all aspects. The following gravitational bodies are included in the force model:

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

- **Relative tolerance**: 1e-15
- **Absolute tolerance**: 1e-15
---

#### `*_lisa[1|2|3]_step_1hour.oem`
Orbit files generated fixed **uniform 1-hour step size**.
This set of files is recommended to be used for data processing.