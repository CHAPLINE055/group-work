
# BIT 2118 --- Scientific Computing

### Group Work Repository

**Python solutions for Tasks 2--21**

Numerical methods · Scientific programming · Data visualization
:::

------------------------------------------------------------------------

## Project Overview

This repository contains Python implementations of the Scientific
Computing group assignment. Tasks 2--20 demonstrate different numerical
methods, while Task 21 applies an ODE method to a real-world cold-chain
medicine transport scenario.

The scripts use example inputs, print numerical results, and generate
plots where required. The code is intentionally provided without inline
comments.

## Getting Started

### Requirements

-   Python 3
-   NumPy
-   SciPy
-   Matplotlib

Install the required libraries:

``` bash
python -m pip install numpy scipy matplotlib
```

Run a task from the project directory:

``` bash
python code/Task_02_numpy_arrays.py
```

Replace the filename to run a different task. Plotting scripts open a
Matplotlib window.

## Tasks Overview

  -----------------------------------------------------------------------
  Tasks                               Topics covered
  ----------------------------------- -----------------------------------
  2--5                                NumPy arrays, vectorization,
                                      floating-point errors, and matrix
                                      algebra

  6--9                                Linear systems, LU decomposition,
                                      iterative methods, and eigenvalues

  10--12                              Root finding, Newton and secant
                                      methods, and nonlinear equations

  13--16                              Interpolation, curve fitting,
                                      numerical differentiation, and
                                      integration

  17--18                              Ordinary differential equations
                                      using Euler's method and SciPy

  19--20                              Optimization and Monte Carlo
                                      simulation

  21                                  Real-world application: cold-chain
                                      medicine transport
  -----------------------------------------------------------------------

## Task 21: Cold-Chain Medicine Transport

The final task applies the ODE method to compare how two medicine
containers respond to temperature changes during a 12-hour journey in a
32 °C environment.

The simulation starts with medicine at 8 °C and compares:

-   **Standard container:** warming rate of 0.18 per hour.
-   **Insulated container:** warming rate of 0.07 per hour.
-   **Temperature limit:** 10 °C.

SciPy's `solve_ivp` calculates the temperature changes over time. The
script displays the final temperatures, estimates when each container
reaches the temperature limit, and plots both results.

The model assumes a constant surrounding temperature and a uniform
warming rate throughout the journey. You can change the parameters in
the script to test different conditions.

## Notes

-   Task 3 compares the execution time of a normal loop and NumPy
    vectorization. Timings depend on the computer used.
-   Tasks 3 and 20 use fixed random seeds to make results reproducible.
-   Several scripts allow input parameters to be changed near the top of
    the file. For example, `step` in Task 17 controls the Euler time
    step, while `simulations` in Task 20 controls the number of Monte
    Carlo samples.

------------------------------------------------------------------------

::: {align="center"}
**BIT 2118 --- Scientific Computing Group Work**
:::
