# TaylorBall

MLB simulation pipeline using historical data to validate simulation probabilities.

## Project summary

TaylorBall implements a multi-stage simulation pipeline that ranges from basic probabilistic simulations to more advanced, data-driven models. The primary goals are:
- Simulate games and seasons using historical player and team statistics
- Estimate and verify the probabilities produced by simulation against real outcomes
- Provide a reproducible environment for experimentation and extension

## Contents

- Jupyter notebooks (primary work): explore the data, run simulations, and visualize results.
- data/ (recommended): data files or small derivatives used by the notebooks. Raw/proprietary datasets are not included — scripts should be used to fetch or reconstruct them.
- docs/ (optional): expanded project documentation or results.
- src/ (optional): helper scripts and modules used by the notebooks.

Note: This repository currently consists primarily of Jupyter Notebooks.

## Project stages

1. Basic — simple game-level simulation using aggregated probabilities (e.g., batting average, slugging).
2. Intermediate — player-level simulations with lineups, substitutions, and basic situational modeling.
3. Advanced — richer models (e.g., plate-appearance models, pitch-level features, Bayesian updating) and stricter validation versus historical outcomes.

## Getting started

Prerequisites
- Python 3.8+ recommended
- Git
- JupyterLab or Jupyter Notebook
