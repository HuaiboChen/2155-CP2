## City Zoning Challenge Problem

In this challenge problem, you are an urban planner zoning a growing city. Each city layout is a 7x7 grid where every cell is one of five districts (Residential, Industrial, Commercial, Park, Office). Four advisors (Wellness, Tax, Transportation, Business) each rate layouts on a 0-1 scale, but they have only rated a small fraction of the provided dataset.

Your task: submit 100 city grids that every advisor rates at least 0.75, while making the set as diverse as possible. You will need to predict advisor ratings from limited labels, then select or generate designs that are both valid and diverse. Full details and a baseline solution are in `starter_notebook.ipynb`.

## Files
- `starter_notebook.ipynb`: problem description, scoring explanation, and a baseline solution. Start here.
- `utils_public.py`: helper functions for loading data, plotting grids, and computing the diversity score.
- `datasets/grids_*.npy`: 500,000 city grids (split across 5 files; load them with `load_grids()`).
- `datasets/scores.npy`: advisor ratings for the grids. Each advisor has rated 5,000 grids; all other entries are NaN.
- `assets/`: images used by the notebook and plotting functions.

## Python Requirements
First create a new environment in conda/mamba:

```bash
conda create --name CP2 python=3.10
```

Then activate the environment and install packages using pip:

```bash
conda activate CP2
pip install -r requirements.txt
```

## Submission
Submit a single `.npy` file containing a 100x7x7 integer array with values from 0 to 4. The end of the starter notebook shows how to check the format and save your submission to the `submissions/` folder.
