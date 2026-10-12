# Ethylene–Isobutane to N-Octane | Aspen Plus V11

## About the Project

This is one of my chemical engineering simulation projects, built using Aspen Plus V11.

I wanted to get more practical experience with process simulation and understand how different equipment works together in a chemical plant. For this project, I built a simplified process model involving ethylene, isobutane, and n-octane.

The simulation includes a reactor, cooler, flash separator, distillation column, and recycle streams. I also studied how changing the reactor outlet temperature affects some of the process results.

This project is part of my journey towards becoming a better chemical engineer, especially in process engineering, energy, and industrial optimisation.

## Tools Used

- **Aspen Plus V11:** For building and running the process simulation.
- **WPS Spreadsheets:** For organising simulation results and plotting graphs.
- **GitHub:** For documenting the project and sharing my work.

## The Process

The process starts with fresh ethylene and isobutane feeds. These are mixed with the recycle streams before entering a heater and then the reactor.

After the reactor, the stream is cooled and sent to a flash separator, where it is divided into vapour and liquid phases.

The liquid stream enters a distillation column. The column separates the feed into an overhead stream and a bottoms product stream. Part of the overhead stream is recycled, while the remaining portion is purged from the process.

The main equipment in the flowsheet includes:

- **Mixer:** Combines the fresh feeds and recycle streams.
- **Heater:** Raises the feed temperature before the reactor.
- **Reactor:** Represents the specified chemical conversion.
- **Cooler:** Lowers the reactor outlet temperature.
- **Flash separator:** Separates the stream into vapour and liquid phases.
- **Distillation column:** Separates the liquid feed into overhead and bottoms streams.
- **Splitter:** Divides the overhead stream between recycle and purge.

## Flowsheet

![Aspen Plus Process Flowsheet](flowsheet.png)

*The flowsheet screenshot will be displayed here once uploaded.*

## Reaction Model

The simulation uses the following simplified reaction:

\[
2C_2H_4 + C_4H_{10} \rightarrow C_8H_{18}
\]

In this model, ethylene and isobutane are the reactants, while n-octane is the intended product.

I used an RStoic reactor in Aspen Plus and specified an ethylene conversion of 80%.

**A note on the chemistry:** This is a simplified stoichiometric model for learning process simulation. It does not establish that the reaction proceeds through this pathway under real industrial conditions, and the model does not predict reaction kinetics.

## Main Simulation Settings

These are the operating conditions used for the base case.

| Parameter | Value |
|---|---:|
| Fresh ethylene feed | 100 kmol/h |
| Fresh isobutane feed | 50 kmol/h |
| Feed temperature | 25 °C |
| Feed pressure | 10 bar |
| Reactor outlet temperature | 100 °C |
| Reactor pressure | 10 bar |
| Specified ethylene conversion | 80% |
| Flash separator temperature | 20 °C |
| Flash separator pressure | 10 bar |
| Light-stream recycle | 95% |
| Light-stream purge | 5% |
| Distillation column stages | 15 |
| Column feed stage | 3 |

The property method used for the simulation is Peng–Robinson.

## Temperature Sensitivity Study

One of the things I investigated was how the reactor outlet temperature affects the rest of the process.

I ran cases at five temperatures:

**60 °C, 80 °C, 100 °C, 120 °C, and 140 °C.**

I then compared five process variables:

- N-octane component flow
- Cooler duty
- Flash liquid flow
- Flash vapour flow
- Reboiler duty

I organised the results in WPS Spreadsheets and plotted the graphs to make the changes easier to compare.

### 1. Effect of Temperature on N-Octane Production

![Effect of Temp on N-Octane Production](sensitivity-analysis/Effect%20of%20Temp%20on%20N-Octane%20Production.png)

The calculated n-octane component flow remained almost constant across the five temperature cases.

This is worth noting, but it needs to be interpreted in the context of the model: the reactor conversion was specified at 80%, rather than calculated from temperature-dependent reaction kinetics.

### 2. Effect of Temperature on Cooler Duty

![Effect of Temp on Cooler Duty](sensitivity-analysis/Effect%20of%20Temp%20on%20Cooler%20Duty.png)

This was one of the clearest changes in the study.

The reported cooler duty became more negative as the reactor outlet temperature increased. In Aspen Plus, this generally indicates that more heat is being removed from the process.

The result shows how the temperature selected for the reactor outlet can affect the cooling requirement in this particular simulation.

### 3. Effect of Temperature on Flash Liquid Flow

![Effect of Temp on Liquid Flow](sensitivity-analysis/Effect%20of%20Temp%20on%20Liquid%20Flow.png)

The flash liquid flow changed only slightly across the temperatures investigated.

The differences are small, so the actual numerical values are more useful than judging the trend from the graph alone.

### 4. Effect of Temperature on Flash Vapour Flow

![Effect of Temp on Vapour Flow](sensitivity-analysis/Effect%20of%20Temp%20on%20Vapour%20Flow.png)

The flash vapour flow also remained almost constant.

This suggests that the change in reactor outlet temperature had little effect on the calculated vapour flow under the selected simulation conditions.

### 5. Effect of Temperature on Reboiler Duty

![Effect of Reactor Temperature on Reboiler Duty](sensitivity-analysis/Effect%20of%20Reactor%20Temperature%20on%20Reboiler%20Duty.png)

The reboiler duty showed very little variation across the five cases.

In this model, the temperature changes had a much more noticeable effect on cooler duty than on reboiler duty.

## What I Learned

Working on this project gave me practical experience with:

- Building a process flowsheet in Aspen Plus.
- Setting up a stoichiometric reactor.
- Connecting flash separation and distillation operations.
- Working with recycle and purge streams.
- Running temperature sensitivity cases.
- Comparing stream flow rates and equipment duties.
- Organising simulation results and presenting them as graphs.

It also reminded me that simulation results should not be accepted without understanding the assumptions behind them.

## Files in This Project

- `README.md` — overview of the project and its results.
- `flowsheet.png` — screenshot of the Aspen Plus flowsheet.
- `data/` — documentation and numerical sensitivity-study data.
- `results/` — simulation results and supporting files.
- `sensitivity-analysis/` — the five graphs from the temperature study.

## Limitations and What I Want to Improve

This is still a learning project, so there are things I would like to investigate further.

The reactor uses a specified conversion rather than a kinetic model. The reaction itself is also a simplified representation and has not been validated against experimental data.

I would like to explore different recycle and purge settings, examine the material and energy balances more closely, and investigate more realistic reaction models where suitable literature and data are available.

These improvements would help me understand not just how to build a simulation, but also how to judge whether its results are physically meaningful.

---

**This project is part of my ongoing learning in chemical engineering, with a particular interest in process simulation, energy systems, and industrial process improvement.**
