# README

This directory contains *dispersed sample orbit files* derived from the nominal orbit files in the parent directory.  
Only a limited set of **30 samples** is provided here, corresponding to the **worst‑case absolute arm‑length rate difference scenarios**.

The following dispersion sources are included, consistent with **CReMA 2.0, Section 6.4**:

---

### • Navigation dispersion from the cartwheel insertion manoeuvre sequence  
This includes uncertainties introduced during the full insertion sequence, including:
- Xenon venting  
- The final MPS manoeuvre  

These dispersions reflect the expected navigation errors accumulated during the cartwheel insertion.

---

### • Stochastic self‑gravity–induced acceleration (Requirement **R‑MIS‑2120**)  
A stochastic propulsive acceleration is added to represent the self‑gravity‑induced effects during science operations.  
Because the self‑gravity field will not be perfectly known at the moment of cartwheel orbit insertion, a residual unmodelled acceleration is always expected throughout the science orbit.

---

### • Parasitic Δv from safe modes and DFACS outages (Requirement **SRD‑MIS‑0040**)  
Parasitic Δv due to safe‑mode entries and DFACS interruptions is modelled as a *constant random acceleration* along the local orbital axes.

It is assumed that the maximum allowed Δv budget of:

- **0.5 cm/s** (along‑track)  
- **1.0 cm/s** (cross‑track)  
- **1.0 cm/s** (radial)

is accumulated *linearly* over the duration of the NSP.

This corresponds to constant acceleration levels of up to:

- **3.52 × 10⁻¹¹ m/s²** (along‑track)  
- **7.04 × 10⁻¹¹ m/s²** (cross‑track)  
- **7.04 × 10⁻¹¹ m/s²** (radial)

Each component follows a uniform random distribution within these bounds.

---
