# AMOC Tipping Analysis Using FitzHugh–Nagumo Models and NGRIP Ice-Core Data

This project explores **FitzHugh--Nagumo--type dynamical systems** and
applies them to paleoclimate data from the **NGRIP δ¹⁸O ice-core
record**. The workflow involves symbolic derivations, numerical
integration, phase-space analysis, parameter optimization, and
evaluation of tipping-point statistics.

The project is implemented as a single Jupyter Notebook (`main.ipynb`)
containing all components of the analysis.

## Project Overview

### 1. FitzHugh--Nagumo Dynamical System

The notebook begins by defining a two-variable nonlinear dynamical
system inspired by the FitzHugh--Nagumo excitable-system model. The
workflow includes:

-   Symbolic derivation of the **Jacobian matrix** and **partial
    derivatives** using *SymPy*
-   Construction of numerical dynamical functions for simulation
-   Visualization of:
    -   Trajectories
    -   Isoclines
    -   Vector fields
    -   Equilibrium points
    -   Complete phase diagrams

These steps establish a mathematical and qualitative understanding of
system behavior.

### 2. NGRIP δ¹⁸O Climate Proxy Analysis

The second part analyzes paleoclimate data:

-   Import of the **NGRIP O¹⁸ dataset**
-   Preprocessing and visualization
-   Estimation of **noise characteristics** using an **AR(1) model**

This section connects the theoretical dynamical system to real-world,
noisy climate observations.

### 3. Model--Data Integration

The notebook combines the FitzHugh--Nagumo model with the proxy
measurements:

-   Definition of a cost/likelihood function
-   Parameter calibration
-   Optimization of key model parameters (**a, b, c, d**) to best match
    observation statistics
-   Visualization of model--data differences

This produces a calibrated dynamical model consistent with the empirical
climate record.

### 4. Tipping-Point Statistics

The project analyzes tipping behavior by:

-   Running simulations with optimized parameters
-   Extracting distributions of tipping intervals or amplitudes
-   Comparing model statistics with the NGRIP record

The analysis highlights whether the FitzHugh--Nagumo type system can
reproduce tipping phenomena observed in paleoclimate.

### 5. Additional Figures

The notebook concludes with extra visualization routines used for
supporting analysis, publication, or presentation.

## Technologies Used

-   **Python**, Jupyter Notebook
-   **NumPy**, **SciPy**
-   **SymPy**
-   **Matplotlib**
-   **pandas**
-   Other helper/utilities

## How to Run

1.  Install dependencies:

    ``` bash
    pip install numpy scipy sympy matplotlib pandas
    ```

2.  Open the notebook:

    ``` bash
    jupyter notebook main.ipynb
    ```

3.  Run all cells from top to bottom.

## Applications

-   Paleoclimate modeling\
-   Early-warning indicators and tipping points\
-   Nonlinear dynamical systems\
-   Excitable media applications\
-   Research in climate dynamics
