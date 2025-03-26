# 🧮 Simulation of Riemann-Liouville Fractional Brownian Motion

## 🎯 Project Objective

This project focuses on simulating the Riemann-Liouville fractional Brownian motion (fBm), a stochastic process with memory and self-similarity properties. The goal is to implement and compare different numerical schemes for path generation, particularly in the low Hurst exponent regime.

## 🧠 Background

The fractional Brownian motion used here is defined through a specific integral representation involving a time-dependent kernel. Its covariance structure is non-trivial and is studied in detail to ensure accurate simulation. We also explore how the process behaves for different ranges of the Hurst parameter (H), especially when H is less than 0.5.

## ⚙️ Methodology

- Analysis of the covariance kernel and its mathematical properties.
- Derivation of a closed-form expression for the covariance when possible.
- Validation of the model for different values of the Hurst exponent.
- Implementation of several simulation methods:
  - Cholesky decomposition (used as a reference)
  - Euler-based schemes
  - Multifactor approximations

## 📏 Evaluation

Two main evaluation metrics are considered:
- **Accuracy:** How close the simulated paths are to the reference Cholesky paths.
- **Efficiency:** Computation time required to generate each sample path.

The error is measured using the Mean Squared Error (MSE) between methods, and the runtime is benchmarked using Python's `timeit` module.

## 📊 Visualization

The notebook includes path visualizations to compare different methods using the same Gaussian noise. These comparisons help highlight trade-offs between computational speed and simulation precision.

## 🧪 Tools & Libraries

- Python
- NumPy & SciPy
- Matplotlib
- Timeit for benchmarking

## ✅ Outcomes

This project provides insight into efficient simulation of fractional Gaussian processes. It highlights the numerical challenges that arise when simulating processes with long memory and proposes practical solutions adapted to different use cases.

## 👤 Author

Philippe YAO – January 2025
