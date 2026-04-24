Numerical Design and Performance Mapping of a Micro Cold-Gas Thruster
 Overview

This project focuses on the development of a quasi-one-dimensional numerical solver to simulate compressible flow through converging–diverging nozzles for micro cold-gas thruster applications.

The solver is designed to efficiently capture key flow phenomena such as:

Transonic acceleration
Shock wave formation
Supersonic expansion

It provides a computationally efficient alternative to full CFD, while maintaining high accuracy for preliminary propulsion design.

Objectives
Develop a finite-volume based solver for quasi-1D Euler equations
Implement and compare multiple numerical schemes
Accurately capture shock discontinuities and expansion physics
Validate results using:
Analytical isentropic relations
ANSYS Fluent simulations
Perform parametric performance analysis for micro-thrusters

Methodology
Governing Model
Quasi-one-dimensional compressible Euler equations
Conservative formulation with geometric source term
Numerical Approach
Finite Volume Method (FVM)
Explicit time integration using Runge-Kutta schemes
CFL-based stability control
Implemented Schemes
Lax–Friedrichs (baseline, diffusive)
HLLC (shock-resolving Riemann solver)
MUSCL–HLLC (second-order, high accuracy with TVD limiter)

The MUSCL–HLLC scheme with MinMod limiter provided the best balance between accuracy and stability.

Key Results
Accurate prediction of:
Mach number distribution
Pressure variation
Shock location
Validation results show strong agreement:
Analytical comparison error ≈ 2–6%
CFD comparison MAPE ≈ 12.6%
Clear identification of flow regimes:
Fully subsonic
Shock-containing
Fully supersonic
⚙️ Performance Insights

The solver was used to evaluate propulsion performance:

Helium
Higher specific impulse (~244 s)
Lower thrust
Nitrogen
Higher thrust (~495 mN)
Lower specific impulse

This demonstrates the classical propulsion trade-off between efficiency and thrust.

Validation Strategy
Analytical validation using isentropic relations
Shock validation using normal shock theory
CFD comparison using ANSYS Fluent (2D axisymmetric model)

Team
Tanuj Sidhwa
Tejas Bhavekar
Siddharth Vezzu
Sudarsanam Sai Sri Narasimha

Future Work
Extend to 2D/axisymmetric solvers
Incorporate viscous effects (Navier–Stokes)
Couple with optimization frameworks for design automation
Integrate with AI-based surrogate models
Key Takeaway

This project demonstrates that a well-designed quasi-1D solver can:

Capture essential compressible flow physics
Resolve shocks accurately
Provide fast and reliable performance estimates

making it a powerful tool for early-stage propulsion system design.
