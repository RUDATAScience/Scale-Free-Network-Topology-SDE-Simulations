# Thermodynamic Limit & Topological Hysteresis SDE Simulations

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## Overview
This repository contains a highly optimized Stochastic Differential Equation (SDE) simulation framework designed to evaluate topological phase transitions, systemic cascades, and high-dimensional algorithmic interventions within scale-free networks. 

The simulations mathematically validate complex network vulnerabilities, specifically addressing targeted hub attacks, macroscopic sensor failures via thermodynamic shielding, and the critical temporal windows required for topological restoration. The framework scales up to **10,000,000 nodes ($10^7$)**, explicitly verifying asymptotic stability and scale invariance at the thermodynamic limit.

## Key Features & Mathematical Proofs
This project consists of three core hypotheses and an extended massive-scale verification phase:

### 1. Hypothesis 1: Irreversible Topological Hysteresis
- **Mechanism:** Simulates the systemic propagation of topological defects ($\beta_1$) when a malicious payload targets structural hubs.
- **Finding:** Demonstrates that removing the attack payload ($b_t = 0$) does not reverse the macroscopic defect. The network enters an irreversible hysteresis plateau.

### 2. Hypothesis 2: Thermodynamic Shielding & Sensor Failure
- **Mechanism:** Evaluates the robustness of aggregate mean-field sensors ($X_A$) against noise flooding attacks ($\lambda_{dummy}$).
- **Finding:** Proves that massive dummy data injection artificially dilutes the macroscopic sensor below detection thresholds ($\theta = 0.18$), completely masking a severe, ongoing systemic collapse ($\beta_1 \approx 0.696$).

### 3. Hypothesis 3: High-Dimensional Interventions & Latency
- **Mechanism:** Compares the restorative efficacy of 1D edge injections versus 2D simplex (triad) injections.
- **Finding:** Mathematically validates that low-dimensional (1D) interventions actively exacerbate topological porosity. Only high-dimensional (2D) interventions suppress the defect, provided they are executed within a strict temporal window (a 50-step delay incurs a permanent $+0.0071$ defect penalty).

### 4. Thermodynamic Limit Verification ($N \to 10^7$)
- **Ergodic Self-Organization:** Utilizes the Kolmogorov-Smirnov statistic ($D_{KS}$) to prove that the system self-organizes independently of arbitrary initial conditions (decaying to $\approx 0.010$).
- **Scale Invariance:** Validates asymptotic stability across 6 logarithmic scales ($N=10^3$ to $10^7$), proving that the partial derivative $\frac{\partial \beta_1}{\partial \log N}$ converges to $\approx 0$, rendering micro-level empirical calibration mathematically unnecessary.

## Requirements & Environment
The computational engine utilizes **Numba** for in-place JIT compilation, ensuring ultra-fast and memory-efficient execution capable of handling 10-million-node adjacency approximations within standard hardware constraints (e.g., Google Colab free tier).

- `numpy`
- `pandas`
- `scipy`
- `matplotlib`
- `numba`

## Usage
The simulation scripts are structured to run seamlessly in Jupyter Notebooks or Google Colab environments.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/RUDATAScience/Network-Topology-Stochastic-Differential-Equation-SDE-Simulations.git](https://github.com/RUDATAScience/Network-Topology-Stochastic-Differential-Equation-SDE-Simulations.git)
   cd Network-Topology-Stochastic-Differential-Equation-SDE-Simulations
