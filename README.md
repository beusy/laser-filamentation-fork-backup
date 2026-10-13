# Femtosecond Laser Filamentation in Fused Silica

Numerical study of nonlinear pulse propagation, self-focusing, and plasma-mediated intensity clamping at a carrier wavelength of 800 nm.

## Overview

This work investigates how diffraction, dispersion, Kerr nonlinearity, and ionisation govern the propagation of an ultrashort laser pulse in fused silica. A cylindrically symmetric envelope model resolves the coupled evolution of the optical field and free-electron density in the single-filament regime.

The accompanying notebook contains the numerical implementation, component validation, and propagation diagnostics. The report develops the physical model and discusses the numerical results.

## Physical model

A generalized nonlinear Schrödinger equation for the field envelope is coupled to a plasma rate equation in the retarded-time frame. The model includes:

- Radial diffraction and group-velocity dispersion.
- Kerr self-focusing and self-phase modulation.
- Multiphoton absorption and ionisation.
- Plasma defocusing and inverse-Bremsstrahlung absorption.
- Avalanche ionisation and recombination.

The cylindrical symmetry and paraxial envelope approximation restrict the scope to single-filament propagation; transverse symmetry breaking and multiple filaments are outside this model.

## Numerical methods

Propagation uses a symmetric split-step scheme, combining Fourier-domain dispersion with Crank–Nicolson radial diffraction. The plasma rate equation is integrated along retarded time, and an absorbing outer radial region limits boundary reflections.

Validation cases include Gaussian-beam diffraction, dispersive pulse broadening, subcritical Kerr propagation, and multiphoton absorption. Diagnostics track peak intensity, electron density, beam width, pulse energy, temporal evolution, and spectral structure.

## Report and implementation

| Resource | Contents |
|---|---|
| [Report](./Laser_Filamentation__Nonlinear_Self_Channeling_of_Light.pdf) | Physical formulation, numerical analysis, and discussion |
| [Simulation notebook](./filamentation_v1%20Final.ipynb) | Solver, validation cases, and propagation calculations |

## Running the notebook

The implementation uses Python with NumPy, SciPy, and Matplotlib, in a Jupyter environment. Open the simulation notebook and execute its cells in order. Material parameters, pulse settings, and grid resolution are defined near the beginning of the notebook. Full propagation calculations can be computationally intensive.

## Authors

Mayad Mnif · Don van Beusichem · Nayl Poirot · Marc Obeid  
École Polytechnique

This repository presents the authors' collaborative computational study. The original shared implementation and report are available in the [collaborative repository](https://github.com/MarcObeid06/Laser-Filamentation-Nonlinear-Self-Channeling-of-Light).
