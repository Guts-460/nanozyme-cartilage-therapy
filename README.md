# nanozyme-cartilage-therapy

This repository contains coarse-grained (CG) molecular dynamics simulation data, analysis scripts, and representative structures for the manuscript:

**"Positively and Negatively Charged Metal Nanozymes for Articular Cartilage Therapy"**

## Repository Structure
├── tprs/ # Production simulation parameter files (.tpr) <br>
├── Density_of_GAGs/ # Density of simulated cartilage CG models <br>
├── MD_Convergence/ # Simulations convergence <br>
├── Representative/ # Representative CG structures (PDB format) <br>
└── README.md

## Requirements

- **GROMACS** (version 2022.5 or later recommended)  
  Installation: [https://www.gromacs.org/download.html](https://www.gromacs.org/download.html)
  
## Reproducing Production Trajectories

All production simulation `.tpr` files are located in the `tprs/` directory. To reproduce any trajectory, use:

```bash
gmx mdrun -v -deffnm OUTPUT_PREFIX -s path/to/file.tpr
