# Metroidvania Research

**Read the paper: https://redstoneweewee.github.io/metroidvania-research/**

A concise research brief based on 250 popular metroidvanias and close relatives. It explains a **deep-sea heat metroidvania**, six other ideas, why they are worth prototyping, and how they were compared. About an eight-minute read.

The 17 October 2026 revision gives every core swim move a heat attack, introduces pulling vents and pushing current generators, and separates world pressure valves from reusable player abilities. It includes the design tradeoffs and a recomputed ranking: 3rd of seven developed concepts, unchanged because the model's broad feature annotations are unchanged.

The chart shows comparison scores and error ranges, increasing from left to right. Scores rescale the original model output: 50 is the mean held-out prediction for the selected Steam games, and 10 points is one standard deviation. They are relative units, not percentages or review forecasts. The model was trained on selected popular games and cannot estimate a new release's expected results or its chance of becoming a hit.

## Contents

- `index.html`: the paper, self-contained (charts, data and sketch are embedded)
- `data/games.csv`: all 250 games with every annotated design dimension
- `data/paper_stats.json`: cross-validated predictions, concept scores and bootstrap rank stability

## Sources

Steam store and review APIs and SteamSpy (accessed 16 October 2026); console sales from VGChartz, Nintendo and press reports. Built for ECE 184 with Python (scikit-learn, UMAP).
