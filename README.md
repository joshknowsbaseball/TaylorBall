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

Quick setup (minimal):
```bash
# clone the repo
git clone https://github.com/joshknowsbaseball/TaylorBall.git
cd TaylorBall

# create and activate a virtual environment (macOS / Linux)
python -m venv venv
source venv/bin/activate

# on Windows (PowerShell)
python -m venv venv
.\venv\Scripts\Activate.ps1

# install dependencies (if a requirements.txt is added)
pip install -r requirements.txt

# or install minimal tools manually
pip install jupyterlab pandas numpy matplotlib scipy seaborn

# start Jupyter
jupyter lab
```

Open the notebooks in the repository and run the cells in order. Notebooks are organized to progress from exploration to modeling; run earlier notebooks first to prepare any derived data used later.

Running on Binder or Colab
- Add a `requirements.txt` or `environment.yml` and a Binder badge to enable one-click execution.
- Notebooks can also be opened directly in Google Colab using the "Open in Colab" link if added.

## Data

- This repo does not include proprietary MLB data.
- Recommended open sources:
  - Lahman Baseball Database (batting, fielding, historical team/player records)
  - Retrosheet (play-by-play event data)
  - Statcast (via community packages; check licensing)
- Place cleaned or derivative datasets in a `data/` directory and add a `data/README.md` that documents sources, download instructions, and licensing/attribution.
- Do NOT commit large proprietary files or raw datasets if they violate terms of service — prefer scripts that download or reconstruct data.

## Reproducibility & recommendations

To make this project easier to run and reuse, consider adding:
- `requirements.txt` or `environment.yml` (conda) with pinned versions
- Small `data/README.md` explaining how to obtain or reconstruct datasets
- `src/` directory for reusable functions and unit tests under `tests/`
- GitHub Actions workflow to run lightweight checks (e.g., linting, unit tests)
- Binder/Colab badges for interactive execution
- A LICENSE file (MIT recommended for code; choose an appropriate data license for datasets)

## Contributing

Contributions are welcome. Good first steps:
- Open an issue describing the change
- Create a branch and submit a pull request with tests/documentation as needed

## License

If you do not yet have a license, add one. MIT is a common choice for code. Be explicit about data licensing in `data/README.md`.

## Contact

If you’d like feedback on changes or want me to:
- push this README as a PR,
- add a starter `requirements.txt`, or
- scaffold `data/README.md` and a simple GitHub Actions workflow

tell me which you'd like and I’ll prepare the next change.

