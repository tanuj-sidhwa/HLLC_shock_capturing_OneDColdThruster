# 🚀 Numerical Design and Performance Mapping of a Micro Cold-Gas Thruster

## 📌 Overview
This project focuses on the development of a **quasi-one-dimensional numerical solver** to simulate compressible flow through converging–diverging nozzles for **micro cold-gas thruster applications**.

The solver captures key flow phenomena such as:
- Transonic acceleration  
- Shock wave formation  
- Supersonic expansion  

It serves as a **computationally efficient alternative to full CFD**, while maintaining high accuracy.

---

## 🎯 Objectives
- Develop a **finite-volume solver** for quasi-1D Euler equations  
- Implement and compare numerical schemes  
- Capture **shock discontinuities and expansion physics**  
- Validate using analytical relations and CFD  
- Perform **parametric performance analysis**  

---

## 🧠 Methodology

### Governing Model
- Quasi-1D compressible Euler equations (conservative form)

### Numerical Approach
- Finite Volume Method (FVM)  
- Explicit Runge-Kutta time integration  
- CFL-based time stepping  

### Schemes Implemented
- **Lax–Friedrichs** → robust but diffusive  
- **HLLC** → better shock resolution  
- **MUSCL–HLLC** → second-order accurate with TVD limiter  

**Best performing:** MUSCL–HLLC (MinMod limiter)

---

## 📊 Key Results
- Accurate prediction of Mach number, pressure, and velocity  
- Strong agreement with analytical solutions (~2–6% error)  
- CFD comparison error ~12%  

Flow regimes successfully captured:
- Fully subsonic  
- Shock-containing  
- Fully supersonic  

----

## ⚙️ Performance Insights
- **Helium**
  - Higher specific impulse (~244 s)  
  - Lower thrust  

- **Nitrogen**
  - Higher thrust (~495 mN)  
  - Lower specific impulse  

➡️ Demonstrates thrust vs efficiency trade-off in propulsion

---

## 🧪 Validation
- Analytical (isentropic + shock relations)  
- CFD (ANSYS Fluent, 2D axisymmetric)  

---



## 📄 Documentation
- Mid Evaluation Report  
- Final Project Report  
- Presentation Slides  

---

## 👥 Team
- Tanuj Sidhwa  
- Tejas Bhavekar  
- Siddharth Vezzu  
- Sudarsanam Sai Sri Narasimha  

---

## 🚀 Future Work
- Extend to 2D / axisymmetric solver  
- Include viscous effects (Navier–Stokes)  
- Add optimization framework  
- Explore AI-assisted design  

---

## 📌 Key Takeaway
A quasi-1D solver can efficiently capture compressible flow physics and shock behavior, making it highly useful for **preliminary propulsion design and rapid iteration**.
