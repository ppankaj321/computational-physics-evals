
---

# 📘 Evaluation Task 1 (OpenAI-Evals Style)

## `evals/poisson_2d_eval.md`

```markdown
# Evaluation: 2D Poisson Solver with Spatially Varying Permittivity

## Objective
Assess the ability to translate a physical electrostatics problem into a
numerically stable, verifiable Python implementation.

## Problem
Solve the 2D Poisson equation:

∇·(ε(x,y) ∇φ) = −ρ(x,y)

on a rectangular domain representing a semiconductor heterostructure.

## Requirements
- Finite difference discretization (≥ 2nd order)
- Dirichlet and Neumann boundary conditions
- Sparse linear solver
- Grid convergence study
- Visualization of φ and E fields

## Evaluation Signals
The solution is considered correct if:
- Numerical residual decreases with grid refinement
- Boundary conditions are correctly enforced
- Electric field shows physically consistent behavior
- Code is readable, modular, and documented

## Failure Modes
- Dense matrix assembly
- Boundary leakage artifacts
- Lack of convergence analysis
