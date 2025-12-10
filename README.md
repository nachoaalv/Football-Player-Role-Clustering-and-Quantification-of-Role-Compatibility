# Football Player Role Clustering and Quantification of Role Compatibility

This repository accompanies my dissertation. It includes Jupyter notebooks, processed data outputs, figures, and the final PDF. This project introduces a role-based framework for tactical analysis and lineup optimisation in football. Using season-long data, players are clustered into roles and evaluated through synergy matrices that measure how combinations affect team output across metrics like xG, pressures, and win rate. In addition, a lineup optimiser builds full XIs based on selected metrics and formation constraints. The system is adaptable to any season dataset and supports applications in recruitment, tactical planning, and match preparation. Future work includes match simulation, squad-based optimisation, and real-world validation. All data was from Laliga, Premier League, Bundesliga, Serie A and Ligue1 2015/16 season.

## Data source
This project uses football event data from the StatsBomb Open Data repository:
- https://github.com/statsbomb/open-data
- License: https://github.com/statsbomb/open-data/blob/master/LICENSE.md

Raw StatsBomb data is not redistributed here; only processed outputs derived for academic purposes are included.

## Contents
- `notebooks/` — analysis notebooks (positions, synergy matrices, lineup optimiser)
- `src/dataset_build/` — league-specific data processing scripts
- `data/processed/` — processed datasets (e.g., player features, roles)
- `results/` — synergy matrices and figures
- `dissertation` — full dissertation

## Reproducibility

To reproduce the analysis, you need to:

1. **Download StatsBomb Open Data**  
   - Clone or download from: https://github.com/statsbomb/open-data  
   - Place the raw JSON event files in a local folder (e.g., `data/raw/`).  
   - This repository does not redistribute raw StatsBomb data.

2. **Install dependencies**  
   - Python 3.10+ recommended.  
   - Install required libraries:  
     - pandas
     - scikit-learn
     - matplotlib
     - seaborn
     - umap-learn
     - tqdm

3. **Run the pipeline**  
   - **Dataset build notebooks** (`src/databuild/`) → process raw StatsBomb data into season-long player datasets.  
   - **Position clustering notebooks** (`notebooks/positions/`) → cluster players into roles.  
   - **Synergy matrices notebook** (`notebooks/complimentary matrices final.ipynb`) → generate role compatibility matrices. 
   - **Lineup optimiser notebook** (`notebooks/Final Lineup Optimiser.ipynb`) → build lineups using roles and matrices.

Outputs (processed CSVs, synergy matrices) are stored in `data/processed/` and `synergy_matrices/`.


## License
- Code and notebooks: GPLv3 (see LICENSE file).
- Dissertation (dissertation.pdf): Creative Commons BY-NC 4.0 (see LICENSE-DISSERTATION file).
- Data: Derived from [StatsBomb Open Data](https://github.com/statsbomb/open-data), licensed under the StatsBomb Open Data License. Raw data is not redistributed here.
