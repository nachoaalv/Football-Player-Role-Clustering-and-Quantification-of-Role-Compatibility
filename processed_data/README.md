# Processed Data

This folder contains processed datasets derived from StatsBomb Open Data.  
Raw StatsBomb data is not redistributed here.



### Files
- `cleaned_player_data_<league>_2015_16.csv` — Example player dataset for each league.
- `all_player_roles.csv` — Combined dataset of all leagues with final role assignments.
These datasets were the output of the `dataset build final-<league>.ipynb` notebooks from the `src/dataset_build` folder.

### Roles data
Located in `roles_data/`:
- Position-specific CSVs  
- Each file lists players and their assigned roles.
These datasets were the output of the `<position>.ipynb` notebooks from the `notebooks/positions` folder.
