# Notebooks

This folder contains Jupyter notebooks used for analysis and experimentation.

### Main notebooks
- `Final Lineup Optimiser.ipynb` — Builds lineups using player roles and the user-chosen synergy matrices.
- `synergy_matrices_final.ipynb` — Generates the 11 synergy matrices from processed player data.

### Position clustering notebooks
Located in `positions/`:
- `goalkeepers.ipynb`
- `centerbacks.ipynb`
- `fullbacks.ipynb`
- `wingers.ipynb`
- `strikers.ipynb`
- `midfielders.ipynb` (all midfielders together)
- `midfielders_split.ipynb` (final version, splits midfielders into 4 sub-groups before clustering)

These notebooks cluster players into roles using k-means and dimensionality reduction.
