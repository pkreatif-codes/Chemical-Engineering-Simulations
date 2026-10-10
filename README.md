# Chemical Engineering Simulations

A growing portfolio of chemical engineering simulations, process
modelling studies, thermodynamic analysis, and engineering calculations.

This repository documents my work in chemical process simulation,
process optimization, separation processes, reaction engineering,
thermodynamics, and data-driven engineering.

The objective is to develop a practical understanding of chemical
engineering systems by building process models, analyzing simulation
results, investigating operating conditions, and documenting
engineering decisions.

---

## Areas of Focus

- Chemical process simulation
- Reaction engineering
- Separation processes
- Thermodynamic modelling
- Material and energy balances
- Sensitivity analysis
- Process optimization
- Recycle and purge systems
- Vapor-liquid equilibrium
- Data regression and model validation
- Energy and economic analysis
- AI and machine learning for chemical engineering

---

## Simulation Projects

### 1. Ethylene and Isobutane to Octane

**Software:** Aspen Plus V11  
**Thermodynamic Model:** Peng-Robinson

A simplified process simulation investigating the conversion of
ethylene and isobutane into n-octane.

The flowsheet includes feed mixing, heating, a stoichiometric reactor,
cooling, flash separation, distillation, and material recycle.

The project investigates:

- Material balance and component conversion
- Flash separation performance
- Distillation and product purity
- Recycle and purge configurations
- Sensitivity analysis
- Energy requirements
- Process optimization

The reaction used in the simplified model is:

2 C2H4 + C4H10 -> C8H18

This stoichiometric representation is a simplified modelling
assumption and does not establish the actual industrial reaction
mechanism or kinetics.

**Project status:** Process model developed; further analysis ongoing.

[View project](Aspen-Plus/01-Ethylene-Isobutane-to-Octane/)

---

### 2. Biogas Upgrading and CO2 Removal

**Software:** Aspen Plus

A process simulation investigating the production and upgrading
of biogas, with emphasis on methane recovery and carbon dioxide removal.

Potential areas of investigation include:

- Gas composition
- Separation performance
- Methane recovery
- Carbon dioxide removal
- Material and energy balances
- Process efficiency

**Project status:** Development and analysis.

[View project](Aspen-Plus/02-Biogas-Upgrading/)

---

## Technical Methods

The repository may include:

- Steady-state process simulation
- Material and energy balance calculations
- Parametric and sensitivity studies
- Thermodynamic property modelling
- Regression and experimental data comparison
- Process performance evaluation
- Economic and sustainability assessment

Methods and results will be documented with their assumptions,
limitations, and applicable operating conditions.

---

## Tools and Technologies

- Aspen Plus
- Aspen HYSYS
- MATLAB
- Python
- Excel

Tools listed here are intended areas of use; individual project
documentation identifies the software actually used.

---

## Repository Structure

```text
Aspen-Plus/       Aspen Plus process simulations
Aspen-HYSYS/      Aspen HYSYS projects
MATLAB/           Engineering calculations and numerical models
Python/           Engineering scripts and modelling
Data-Analysis/    Regression and data analysis
docs/             Shared technical documentation
