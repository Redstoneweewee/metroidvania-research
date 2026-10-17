# Metroidvania Research

**Read the paper: https://redstoneweewee.github.io/metroidvania-research/**

A concise research brief based on 250 popular metroidvanias and close relatives. It explains a **deep-sea heat metroidvania**, six other ideas, why they are worth prototyping, and how they were compared. About a nine-minute read, with an interactive design-space map and a searchable game table.

The 17 October 2026 revision follows the author's annotations and confirmed design choices: passive drift and dive, an active short upward kick and horizontal dash, 5–10 second heat trails, enemy fights as the main killing method, and movement that becomes weaker only when heat reaches zero. Hot vents pull, refuel and propel; cool currents push outward. Heat fear remains a possible addition. Bosses and map layers use descriptive labels. The existing model comparison is shown as 3/7; the new enemy interactions have not received new feature ratings.

The chart shows comparison scores and error ranges, increasing from left to right. Scores rescale the original model output: 50 is the mean held-out prediction for the selected Steam games, and 10 points is one standard deviation. They are relative units, not percentages or review forecasts. The model was trained on selected popular games and cannot estimate a new release's expected results or its chance of becoming a hit.

## Contents

- `index.html`: the paper, self-contained (charts, data and sketch are embedded)
- `data/games.csv`: all 250 games with every annotated design dimension
- `data/paper_stats.json`: cross-validated predictions, concept scores and bootstrap rank stability

## Sources

Steam store and review APIs and SteamSpy (accessed 16 October 2026); console sales from VGChartz, Nintendo and press reports. Built for ECE 184 with Python (scikit-learn, UMAP).
