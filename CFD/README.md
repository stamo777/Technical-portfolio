# Formula 1 CAD & CFD Analysis – DRS Rear Wing

## Project Overview

This personal engineering project combines CAD modelling and CFD analysis to investigate the aerodynamic influence of the Drag Reduction System (DRS) on a simplified Formula 1 rear wing.

The Formula 1 car and rear-wing geometries were modelled using **3DEXPERIENCE**, based on reference images and dimensional scaling. Two rear-wing configurations were then investigated using **OpenFOAM**:

- DRS closed
- DRS open

The CFD study focuses on the resulting changes in drag, downforce, pressure distribution and velocity field.

## Tools

- **3DEXPERIENCE** – CAD modelling
- **OpenFOAM** – CFD simulation
- **snappyHexMesh** – Mesh generation and refinement
- **ParaView** – CFD post-processing and visualization
- **ImageJ** – Dimensional scaling from reference images

## CFD Methodology

The simulations were performed at a freestream velocity of **50 m/s** using a steady-state **RANS k-ε turbulence model**.

The workflow included:

- Computational domain definition and boundary-condition setup
- Surface refinement with snappyHexMesh
- Near-wall prism-layer generation
- Mesh-quality assessment
- y+ assessment
- Residual and convergence monitoring
- Pressure and velocity-field analysis
- Aerodynamic force calculation
- Drag-coefficient comparison

The final meshes contained approximately:

- **915,000 cells** – DRS closed
- **894,000 cells** – DRS open

The average y+ value was approximately **135** for both configurations, consistent with the high-Reynolds-number wall-function approach used in the study.

## Key Results

At **50 m/s**, opening the DRS produced:

- **58.3% reduction in drag**
- **86.1% reduction in downforce**

Using a common reference area for both configurations, the drag coefficient changed from approximately:

**Cd = 1.06 → 0.44**

These results illustrate the aerodynamic trade-off produced by DRS opening: a substantial reduction in aerodynamic resistance accompanied by a strong reduction in downforce.

## Full Report

The complete methodology, mesh assessment, CFD results, discussion and limitations are available in the engineering report:

➡️ **[View the full CFD report](Report/Report_F1_project.pdf)**

## Project Scope

This project was developed as part of a personal mechanical engineering portfolio. The geometry and CFD model are intentionally simplified and are intended for comparative aerodynamic analysis rather than high-fidelity prediction of an actual Formula 1 car.
