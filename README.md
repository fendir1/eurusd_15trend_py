# EUR/USD 15-Minute Trend Model

A research project that uses Dukascopy EUR/USD tick data to estimate, once per
minute, the probability that EUR/USD will move **up**, remain **flat**, or move
**down** over the following 15 minutes.

The initial modeling pipeline will compare regularized logistic regression
with a LightGBM multiclass classifier. Evaluation will use chronological,
leakage-aware splits and probability-calibration metrics.

## Project structure

```text
raw_data/          Original Dukascopy downloads (not tracked by Git)
data/interim/      Cleaned and intermediate datasets
data/processed/    Final one-minute modeling datasets
notebooks/         Numbered research notebooks
src/               Reusable Python modules
models/            Trained model artifacts
reports/figures/   Generated charts
reports/tables/    Generated evaluation tables
```

Raw data, generated datasets, model artifacts, secrets, and local Python
environments are excluded from version control.
