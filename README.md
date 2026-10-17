# Metroidvania Research

**Read the paper: https://redstoneweewee.github.io/metroidvania-research/**

An interactive research paper that maps 250 popular metroidvanias and close relatives in a 148-dimension design space, measures what travels with popularity, explores underrepresented combinations, and pitches a **deep-sea heat metroidvania** designed for those gaps.

The 17 October 2026 revision gives every core swim move a heat attack, introduces pulling vents and pushing current generators, and separates world pressure valves from reusable player abilities. It includes the design tradeoffs and a recomputed ranking: 3rd of seven developed concepts, unchanged because the model's broad feature annotations are unchanged.

Concept comparisons show relative ranks and bootstrap rank stability, rather than review-count forecasts. The model was trained on a selected set of popular games and cannot estimate a new release's expected reviews or its chance of becoming a hit.

## Contents

- `index.html`: the paper, self-contained (charts, data and sketch are embedded)
- `data/games.csv`: all 250 games with every annotated design dimension
- `data/paper_stats.json`: cross-validated predictions, concept scores and bootstrap rank stability

## Sources

Steam store and review APIs and SteamSpy (accessed 16 October 2026); console sales from VGChartz, Nintendo and press reports. Built for ECE 184 with Python (scikit-learn, UMAP).
