# Chaos control and schedule of shuttle buses

This repository contains the simulation code and a detailed report analyzing the dynamics of a shuttle bus system, focusing on the emergence and control of deterministic chaos. The work replicates and extends the findings of Takashi Nagatani's model, demonstrating how passenger loading and bus speedup parameters influence system stability and predictability.

## Overview

The project investigates a simplified shuttle bus system operating between an origin and a destination. It explores a feedback loop where passenger boarding delays affect bus speeds and headways, potentially leading to irregular arrival patterns and "bunching" of buses, even without external random influences.

## Simulation

The `simulation.ipynb` Jupyter notebook contains the Python code for simulating the shuttle bus system. It includes:

- A `simulate_buses` function that models bus movements, calculates headways and tour times, and incorporates the loading and speedup parameters.
- Code to generate various plots illustrating:
  - Bifurcation diagrams showing the transition from regular to periodic to chaotic schedules as the loading parameter increases.
  - The effect of symmetric and asymmetric speedup parameters on system stability.
  - Return maps confirming the deterministic nature of the chaos (strange attractors).
  - Mean and RMS values of headways and tour times.
  - Phase diagrams mapping stable and unstable regions in the parameter space of loading and speedup.

## How to Run the Simulation

To run the simulation and reproduce the figures:

1. Ensure you have Python and Jupyter Notebook installed.
2. Install the necessary libraries: `numpy` and `matplotlib`.

   ```bash
   pip install numpy matplotlib
   ```

3. Open the `simulation.ipynb` notebook in a Jupyter environment:

   ```bash
   jupyter notebook simulation.ipynb
   ```

4. Run all cells in the notebook to execute the simulation and generate the plots.

## References

- Nagatani, T. (2006). Chaos control and schedule of shuttle buses. *Physica A: Statistical Mechanics and its Applications, 371*(2), 683-691.

- Meerschaert, M. M. (2013). Chapter 4 - Introduction to Dynamic Models. In: Mathematical Modeling (Fourth Edition). Academic Press, Boston. pp. 115-137. ISBN 978-0-12-386912-8.
