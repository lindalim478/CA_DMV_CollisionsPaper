# CA DMV Autonomous Vehicle Collisions — Prelim Research

Preliminary analysis of California DMV autonomous vehicle (AV) collision and
disengagement reports, combined with demographic (census) context, in support
of dissertation research.

## 🗺️ Interactive crash map

**[▶ Open the interactive AV crash map](https://lindalim478.github.io/CA_DMV_CollisionsPaper/AV_Crash_Map.html)**

Click the link above to explore AV crash locations on an interactive map
(hosted via GitHub Pages).

## Contents

| File | Description |
| --- | --- |
| `CA_DMV_CollisionsDataset.csv` | CA DMV AV collision records enriched with location and census/demographic fields (weather, lighting, roadway conditions, fault, injuries, latitude/longitude, median income, population demographics, etc.). |
| `CA_OLSDMV_Reporting.ipynb` | Analysis of the older CA DMV collision reporting data. |
| `Collisions Diagram.ipynb` | Notebook producing collision diagrams / visualizations. |
| `Disengagements.ipynb` | Analysis of AV disengagement reports. |
| `AV_Crash_Map.html` | Source for the interactive map — [view it live here](https://lindalim478.github.io/CA_DMV_CollisionsPaper/AV_Crash_Map.html). |
| `NHTSA EMS Crashes.xlsx` | Supplementary NHTSA EMS crash data. |

## Getting started

The notebooks use the standard Python data stack. A minimal environment:

```bash
python -m venv .venv
source .venv/bin/activate
pip install jupyter pandas numpy matplotlib folium openpyxl
jupyter lab
```

Open any of the `.ipynb` notebooks and run the cells. The crash map can be
viewed live at the [interactive map link](https://lindalim478.github.io/CA_DMV_CollisionsPaper/AV_Crash_Map.html).

## Data notes

The collision dataset joins DMV-reported AV collisions with U.S. Census
tract/block-level demographics (median age, population, race/ethnicity
breakdown, median income) for spatial and equity-oriented analysis.
