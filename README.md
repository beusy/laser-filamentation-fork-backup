# Laser Filamentation: Nonlinear Self-Channeling of Light

Classical Electrodynamics project by second-year Bachelor students at École Polytechnique.

This project studies the physics of femtosecond laser filamentation and nonlinear self-channeling of light in a transparent Kerr medium, with a focus on the cylindrically symmetric single-filament regime. The goal is to understand how an intense ultrashort laser pulse can self-focus, generate plasma, avoid catastrophic collapse, and propagate as a narrow high-intensity filament.

The physical model is based on a generalized nonlinear Schrödinger equation for the electric-field envelope \(E(r,\tau,z)\), coupled to a Drude-type plasma rate equation for the free-electron density. The simulation includes the main mechanisms responsible for filamentation: radial diffraction, group-velocity dispersion, Kerr self-focusing, multiphoton absorption, plasma generation, plasma defocusing, avalanche ionisation, recombination and inverse-bremsstrahlung absorption.

The numerical method uses a Strang split-step propagation scheme. The linear step combines Fourier-spectral propagation for group-velocity dispersion with a Crank--Nicolson finite-difference scheme for radial diffraction. The nonlinear step is evaluated pointwise and updates the field through Kerr, plasma and absorption contributions, while the plasma density is advanced in retarded time.

The simulations are performed for fused silica at a carrier wavelength of 800 nm. The project reproduces the main qualitative and quantitative signatures of laser filamentation: Kerr-driven self-focusing near the Marburger collapse distance, plasma-mediated intensity clamping, pulse splitting and dynamic replenishment, formation of a narrow plasma channel, and the appearance of conical/X-wave structures in the angular spectrum.

## Repository contents

- `Laser_Filamentation__Nonlinear_Self_Channeling_of_Light.pdf`  
  Final written report for PHY204 Project #17.

- `filamentation_v1 Final.ipynb`  
  Jupyter notebook containing the numerical implementation, validation tests, simulations and figures used in the report.

## Main objectives

1. Identify the minimal physical ingredients required to reproduce filamentation.
2. Implement a stable numerical propagation method for the cylindrically symmetric optical envelope.
3. Interpret the simulated filament in terms of self-focusing, plasma defocusing, dynamic replenishment and conical/X-wave propagation.

## Authors

Mayad MNIF  
Don VAN BEUSICHEM  
Nayl POIROT  
Marc OBEID
