# Laser Filamentation: Nonlinear Self-Channeling of Light

<p align="center">
  <img src="https://img.shields.io/badge/PHY204-Classical%20Electrodynamics-blue" />
  <img src="https://img.shields.io/badge/Topic-Laser%20Filamentation-purple" />
  <img src="https://img.shields.io/badge/Medium-Fused%20Silica-orange" />
  <img src="https://img.shields.io/badge/Wavelength-800%20nm-red" />
  <img src="https://img.shields.io/badge/Code-Jupyter%20Notebook-yellow" />
  <img src="https://img.shields.io/badge/Report-LaTeX-green" />
</p>

## Overview

This repository contains the final report and numerical notebook for **PHY204 Project #17: Laser Filamentation — Nonlinear Self-Channeling of Light**, carried out by second-year Bachelor students at École Polytechnique.

The project studies femtosecond laser filamentation in a transparent nonlinear medium, with a focus on the **single-filament cylindrically symmetric regime**. We model the propagation of an ultrashort laser pulse in fused silica at a carrier wavelength of **800 nm**, and analyse how Kerr self-focusing, diffraction, group-velocity dispersion, multiphoton absorption and plasma generation combine to form a narrow high-intensity filament.

## Physical model

The simulation is based on a cylindrically symmetric generalized nonlinear Schrödinger equation for the electric-field envelope $E(r,\tau,z)$ coupled to a Drude-type plasma rate equation for the free-electron density $\rho(r,\tau,z)$.

The model includes:

- radial diffraction,
- group-velocity dispersion,
- Kerr self-focusing and self-phase modulation,
- multiphoton absorption,
- multiphoton ionisation,
- plasma defocusing,
- avalanche ionisation,
- recombination,
- inverse-Bremsstrahlung plasma absorption.

The goal is to reproduce and interpret the main signatures of laser filamentation: **self-focusing, intensity clamping, plasma-channel formation, pulse splitting, dynamic replenishment and conical/X-wave spectral structure**.

## Repository contents

| File | Description |
|---|---|
| [`Laser_Filamentation__Nonlinear_Self_Channeling_of_Light.pdf`](./Laser_Filamentation__Nonlinear_Self_Channeling_of_Light.pdf) | Final written report |
| [`filamentation_v1 Final.ipynb`](./filamentation_v1%20Final.ipynb) | Jupyter notebook containing the numerical implementation, validation tests and simulations |
| [`.gitignore`](./.gitignore) | Files ignored by Git, including Python/Jupyter temporary files |

## Authors

- Mayad MNIF  
- Don VAN BEUSICHEM  
- Nayl POIROT  
- Marc OBEID  

École Polytechnique — PHY204 Classical Electrodynamics
