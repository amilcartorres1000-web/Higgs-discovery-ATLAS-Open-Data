# Observation of the Higgs Boson Peak in ATLAS Open Data — 4 Leptons Channel
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![ROOT](https://img.shields.io/badge/ROOT-Data%20Analysis-3776AB?logo=cern&logoColor=white)
![matplotlib](https://img.shields.io/badge/matplotlib-Visualization-11557c?logo=matplotlib)
![ATLAS](https://img.shields.io/badge/ATLAS-Open%20Data-black)
![Status](https://img.shields.io/badge/Status-Complete-success)

## Description
This project reproduces one of the most iconic results of the **ATLAS experiment** at the **Large Hadron Collider (LHC)**:  
the observation of the **Higgs boson (H → ZZ* → 4ℓ)** peak around **125 GeV**, using **publicly available ATLAS Run 2 Open Data**.

The goal is to analyze real reconstructed collision data to visualize the invariant mass distribution of four-lepton events, clearly showing the **Higgs boson signal** above the Standard Model background.

---

## Objective
- Access and analyze ATLAS Run 2 (2015–2016) open data.
- Reconstruct the invariant mass of four-lepton events (`m₄l`).
- Identify the **Z boson** peak around 91 GeV and the **Higgs boson** signal near 125 GeV.
- Reproduce the published ATLAS-style histogram using `matplotlib`.

---

## Dataset
**Source:** [ATLAS Open Data — Run 2 2015+2016 proton-proton collisions](https://opendata.cern.ch/record/93924)
! Download all files from this link and copy/page in a new folder "Data" 

| Property | Description |
|-----------|--------------|
| Experiment | ATLAS |
| Data years | 2015–2016 |
| Center-of-mass energy | √s = 13 TeV |
| Channel | Exactly 4 leptons (electrons and muons) |
| Variables used | Four-lepton invariant mass (`m₄l`) |

This dataset is a subset of reconstructed events selected to match the **H → ZZ* → 4ℓ** decay topology.

---

## Methodology
1. **Load and process the dataset**
   - Events with exactly four leptons are selected.
   - Invariant mass `m₄l` is computed using the four-momentum of each lepton.

2. **Histogram creation**
   - Events are binned in `m₄l` from 80 GeV to 170 GeV.
   - Each bin represents the number of events per invariant mass interval.

3. **Visualization**
   - Histogram plotted with `matplotlib` in ATLAS style.
   - Annotated peaks:
     - **Z boson peak (~91 GeV)** — Standard Model background.
     - **Higgs boson peak (~125 GeV)** — signal.
