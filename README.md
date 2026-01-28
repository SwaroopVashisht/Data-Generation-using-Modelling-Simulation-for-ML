# Data Generation using Modelling & Simulation for ML (SimPy)

## Step 1: Simulator Selected
**SimPy** (Python discrete-event simulation library)

## Step 2: Simulation Problem
We simulated an **M/M/1 queue** where customers arrive (rate λ) and are served (rate μ).

## Step 3: Parameters + Bounds
- arrival_rate (λ): 0.2 to 2.0
- service_rate (μ): 0.5 to 3.0 (kept > λ for stability)
- sim_time: 200 to 2000

## Step 4–5: Data Generation (1000 simulations)
For each random parameter set, we recorded:
- avg_wait
- avg_system_time
- avg_queue_length
- utilization

Dataset: `simpy_mm1_dataset.csv`

## Step 6: ML Model Comparison
Target: Predict **avg_wait** from input parameters.

Models compared:
- Linear Regression, Ridge, Lasso, KNN, SVR, RandomForest, ExtraTrees, GradientBoosting

Metrics:
- R², MAE, RMSE, Training Time

## Results
(Insert table screenshot or paste the table from notebook)

Graphs:
- `model_comparison_r2.png`
- `actual_vs_predicted.png`

## Conclusion
Best model: **<best_model_name>**
Reason: Highest R² and low error.

## How to Run
Open notebook in Colab and run all cells.
