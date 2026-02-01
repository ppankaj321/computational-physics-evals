# Evaluation: Stochastic Noise Simulation and PSD Validation

## Objective
Evaluate understanding of stochastic differential equations and spectral analysis.

## Problem
Simulate the Langevin equation:

dI/dt = −I/τ + σξ(t)

and validate the resulting noise spectrum.

## Requirements
- Euler–Maruyama integration
- Correct noise scaling
- FFT-based PSD estimation
- Comparison with analytical Lorentzian spectrum

## Evaluation Signals
- Stability for Δt ≪ τ
- Correct PSD slope at low/high frequency
- Clear discussion of numerical artifacts

## Failure Modes
- Incorrect noise normalization
- Aliasing-dominated PSD
- No analytical comparison
