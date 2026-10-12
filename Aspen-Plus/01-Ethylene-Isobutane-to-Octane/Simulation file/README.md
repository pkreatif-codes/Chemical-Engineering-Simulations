# Aspen Plus Simulation Files

This folder contains the Aspen Plus simulation archive for my n-octane production process model, developed using Aspen Plus V11.

## Simulation File

**File:** `Industrial Production of N-Octane from Ethlylene and Isobutane.apwz`

The archive contains the Aspen Plus simulation project for exploring a simplified ethylene–isobutane reaction system for n-octane production.

## Process Overview

The flowsheet includes:

- Feed mixing and heating
- Stoichiometric reactor (RStoic)
- Flash separation (FLASH2)
- Distillation column (RadFrac)
- Vapour recycle and purge streams

## Simulation Conditions

| Parameter | Value |
|---|---|
| Software | Aspen Plus V11 |
| Property method | Peng–Robinson (PENG-ROB) |
| Fresh ethylene feed | 100 kmol/h |
| Fresh isobutane feed | 50 kmol/h |
| Reactor pressure | 10 bar |
| Specified ethylene conversion | 80% |
| Recycle ratio | 95% |
| Purge ratio | 5% |

## How to Open the File

1. Download the `.apwz` file from this repository.
2. Open Aspen Plus V11 or a compatible version.
3. Open or restore the archive using the appropriate Aspen Plus workflow.
4. Review the components, property method, stream specifications, and unit-operation settings.
5. Run the simulation and compare your results with the main project README.

## Purpose

This project was developed to practise process simulation, reactor modelling, separation processes, recycle configuration, and energy analysis.

## Disclaimer

This is an educational simulation using a simplified stoichiometric reaction model. It is not a validated industrial process design, reaction mechanism, or kinetic model. Results may vary with Aspen Plus versions and simulation settings.
