# Temperature Sensitivity Analysis Data

## Overview

This folder contains the numerical data collected from the
Aspen Plus V11 temperature sensitivity study for the
ethylene–isobutane to n-octane process simulation.

## Study Objective

The objective is to investigate how changes in reactor outlet
temperature affect selected process outputs under specified
simulation conditions.

## Temperature Range

The study investigates five reactor outlet temperatures:

- 60 °C
- 80 °C
- 100 °C
- 120 °C
- 140 °C

## Data Parameters

The dataset is intended to contain the following variables:

| Parameter | Unit |
|---|---|
| Reactor outlet temperature | °C |
| N-octane component flow | kmol/h |
| Flash vapour flow | kmol/h |
| Flash liquid flow | kmol/h |
| Cooler duty | kW |
| Reboiler duty | kW |

## Files

- `temperature-study.csv` — numerical data for the temperature sensitivity study.

## Simulation Conditions

The study uses a specified ethylene conversion of 80%, a reactor
pressure of 10 bar, and a light-stream recycle fraction of 95%
with a 5% purge fraction.

Other operating conditions and model specifications are documented
in the main project README.

## Important Note

The reactor uses a specified stoichiometric conversion rather than
temperature-dependent reaction kinetics. Therefore, the dataset
describes the response of the simulated process under the selected
conditions; it does not independently establish the effect of
temperature on actual reaction kinetics.

All data should be interpreted within the assumptions and limitations
of the Aspen Plus model.
