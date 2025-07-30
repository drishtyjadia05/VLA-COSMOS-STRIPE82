# Study of Radio Transients using COSMOS and STRIPE82 Surveys

**Author**: Drishty B. Jadia  
**Degree Project**: Masters' Thesis, [IIT Kanpur](https://www.iitk.ac.in/) 
**Supervisor**: Prof. [Kunal P. Mooley](https://sites.google.com/view/mooleylab/)  
**Duration**: August 2024 – May 2025 *(Ongoing)*  

---

## Overview

This project explores the dynamic radio sky by analyzing 3 GHz VLA observations from two major sky surveys — **COSMOS** and **STRIPE82**. The goal is to identify and characterize radio transients and variables such as **tidal disruption events (TDEs)**, **gamma-ray bursts (GRBs)**, and **neutron star mergers**. These events provide insight into relativistic outflows, compact objects, and extreme astrophysical environments.

---

## Dataset Summary

- **COSMOS Deep Survey**  
  ~2 deg² field observed with VLA in A & C-array at 3 GHz (2048 MHz bandwidth).  
  110 epochs processed to study long-term radio variability.

- **STRIPE82 Survey**  
  ~270 deg² region observed using the novel **On-the-Fly Mosaicing (OTFM)** mode.  
  First wide-field survey with Jansky VLA to probe transients on day-to-year timescales.

---

## Methodology

### COSMOS Field
- Downloaded raw VLA data from NRAO archive for 110 epochs.
- Calibration using **AIPS** pipeline; fallback CASA script developed for failed epochs.
- Imaging using **CASA** `tclean` with optimized parameters (nterms=2, robust=0.5).
- Mosaicking using **AIPS** `flatn` task; produced 440 mosaics.
- Source detection using **PyBDSF** across all mosaics.
- Catalog generation and light curve construction for variability analysis.

### STRIPE82 Field
- Calibration performed using the **VLASS pipeline** on NRAO servers.
- Manual imaging using **CASA** for full control over OTFM-mode data.
- Custom imaging script under development for improved automation.
- Future steps: Primary beam correction → mosaicking → source detection → light curves.

---

## Progress

- COSMOS:  
  - 80 epochs processed → 320 mosaics analyzed.  
  - Source finding completed; >600 sources detected in typical mosaics.  
  - Light curves under preparation.

- STRIPE82:  
  - VLASS pipeline run successfully on all datasets.  
  - Imaging scripts being customized for OTFM mode.  
  - Calibration and imaging workflow validation underway.

---

## Goals

- Identify and classify radio transients and variable sources.
- Quantify flux variability across epochs.
- Associate candidates with known extragalactic phenomena (e.g., AGNs, TDEs).
- Contribute to understanding jet formation, magnetic fields, and accretion physics.

---

## Tools & Technologies

| Category           | Tools Used                                 |
|--------------------|---------------------------------------------|
| Calibration        | AIPS, CASA, VLASS pipeline                  |
| Imaging            | CASA `tclean`, CARTA, AIPS `flatn`          |
| Source Finding     | PyBDSF                                      |
| Programming        | Python, Bash                                |
| Systems            | Linux, SLURM, NRAO remote servers           |
| Data Formats       | FITS, CSV                                   |
| Visualization      | Matplotlib, Astropy, CARTA                  |

---

## Resources & References

- [Project Report](./VLA_COSMOS_STRIPE82.pdf)
- [DATA](https://data.nrao.edu/portal/)
- [COSMOS Survey](https://cosmos.astro.caltech.edu/page/radio)
- [STRIPE82 Surveys Portal](http://www.tauceti.caltech.edu/stripe82/)
- [VLASS Pipeline for Calibration of STRIPE82 data](./hifv_compression.py)
- [The VLA-COSMOS 3 GHz Large Project: Continuum data and source catalog release](https://www.aanda.org/articles/aa/abs/2017/06/aa28704-16/aa28704-16.html)
- [THE CALTECH-NRAO STRIPE 82 SURVEY (CNSS) PAPER](https://iopscience.iop.org/article/10.3847/0004-637X/818/2/105/meta)

---

## Future Work

- Complete imaging and source finding for STRIPE82.
- Finalize variability analysis and transient candidate classification.
- Prepare manuscripts and poster presentations.
- Integrate additional frequency coverage for spectral index studies.

---

## Contact

> dbjadia052gmail.com 
> [Website](https://drishtyjadia05.github.io)  

---
