# TaylorBall

A reproducible MLB game and season simulation project using historical data. Built as a senior project exploring how statistical modeling can predict player performance and team outcomes.

## What This Project Does

TaylorBall implements **three progressive stages of baseball simulation**:

1. **Stage 1: Simple Probabilistic Model** — Basic win probability using league-average outcomes
2. **Stage 2: Team-Level Adjustments** — Incorporates team offensive and pitching metrics
3. **Stage 3: Player-Level Simulation** — Models individual batter-pitcher matchups using historical stats

Each stage builds on the previous one, with validation comparing simulated seasons against actual historical records.

## Quick Start

### Option 1: pip
```bash
pip install -r requirements.txt
jupyter notebook TaylorBall.ipynb
```

### Option 2: conda
```bash
conda env create -f environment.yml
conda activate taylorball
jupyter notebook TaylorBall.ipynb
```

## Data Sources

This project uses publicly available baseball data:
- [Lahman Database](http://www.seanlahman.com/baseball-archive/statistics/) — Historical statistics from 1871-present
- [Retrosheet](https://www.retrosheet.org/) — Play-by-play game logs

## Key Findings

*(Add 2-3 bullet points summarizing your most interesting results, e.g.:)*
- The Stage 3 model predicted season win totals within X games for Y% of teams
- Run differential proved to be the strongest single predictor of...
- Monte Carlo simulations showed that playoff outcomes have higher variance than...

## Project Context

| | |
|---|---|
| **Type** | Senior Capstone Project |
| **Focus** | Baseball Analytics / Sports Data Science |
| **Tools** | Python, Jupyter, pandas, NumPy, matplotlib |

This project demonstrates end-to-end analytical work: scoping a research question, acquiring and cleaning real-world data, building progressively complex models, and validating results against ground truth.

## Limitations & Future Work

- Current model uses season-level stats; pitch-by-pitch data could improve accuracy
- Simulation assumes independent at-bats (doesn't model hot/cold streaks)
- Could extend to project prospect performance or evaluate trades

## License

MIT License — see [LICENSE](LICENSE) for details.

---

**Author:** Josh Taylor  
**Contact:** [joshknowsbaseball](https://github.com/joshknowsbaseball)
