# SIR Epidemic Model & Spatial Simulation 🦠

A mathematical modeling project implementing the classic SIR (Susceptible-Infected-Recovered)
epidemiological framework, extended with spatial simulations across different population
distributions and city geometries.

## 📐 What It Does

### Part 1 — Differential Equation Models
- **Basic SIR model**: solves the SIR system of ODEs for a fixed population, computing R₀ and Reff
- **Non-constant population model**: extends SIR with birth rate (b), mortality (μ), and vaccination (v) parameters
- **Vaccination program model**: simulates the effect of varying vaccination coverage on infection curves

### Part 2 — Spatial Population Models
Generates 4 city configurations to study how population distribution affects spread:
- Square city with uniform distribution
- Circular city with uniform distribution
- Square city with clustered distribution
- Circular city with clustered distribution

### Part 3 — Agent-Based Simulation
Runs iterative spread simulations across all 4 city types using:
- Euclidean distance-based infection radius
- Random agent movement with normal distribution
- Per-iteration state tracking (S → I → R)
- Animated visualization of disease spread

## 📊 Key Concepts

- R₀ (Basic Reproduction Number) and Reff (Effective Reproduction Number)
- ODE solving with `scipy.integrate.solve_ivp`
- Spatial epidemiology and proximity-based transmission
- Agent-based modeling with stochastic movement

## 🛠 Tech Stack

Python · NumPy · SciPy · Pandas · Matplotlib

## ▶️ How to Run
```bash
pip install numpy scipy pandas matplotlib tabulate
```

Open `SIR_System.ipynb` in Jupyter Notebook and run all cells sequentially.
