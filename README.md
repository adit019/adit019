# U.S. Presidential Election Data Visualization (1976-2020)

A self-contained repository for exploring U.S. presidential election outcomes from 1976 through 2020. It bundles the source data, a reproducible visualization script, and an output directory for generated charts and summary tables. Use it as-is or fork it into your own GitHub account to extend the analysis.

## Repository contents
- `data/elections_1976_2020.csv` — Aggregated election results with popular vote percentages, Electoral College totals, and third-party vote share.
- `scripts/visualize.py` — Generates charts for major-party vote trends, margins, Electoral College outcomes, and third-party vote share. Exports a Markdown summary table to `visualizations/README.md`.
- `visualizations/` — Default output directory for generated PNG charts and the summary table (kept in Git via `.gitkeep`).
- `requirements.txt` — Python dependencies for running the visualization script.

## Quickstart
1. **Create and activate a virtual environment**
   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
3. **Generate charts and summary table**
   ```bash
   python scripts/visualize.py
   ```

All outputs will be written to `visualizations/`. The script is intentionally minimal, so you can adapt it for deeper dives (e.g., state-level analysis, turnout trends, or party flips).

## Publishing to GitHub
1. Create a new repository on GitHub (public or private).
2. Add it as a remote and push this project:
   ```bash
   git init
   git remote add origin git@github.com:<your-username>/<your-repo>.git
   git add .
   git commit -m "Add U.S. presidential election visualization toolkit"
   git push -u origin main
   ```

## Project notes
- The dataset is small (12 election cycles) and uses aggregate national results for clarity.
- Charts use a neutral color palette: blue for Democratic, red for Republican, gray for other/third-party.
- The summary table is regenerated each run to match the dataset.
