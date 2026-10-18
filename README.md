# Metroidvania Research

**Read the paper: https://redstoneweewee.github.io/metroidvania-research/**

A short research brief for a student team. It pitches a **deep-sea heat metroidvania** (a platformer with gravity flipped: you float up, and going deeper means using the terrain), then checks what's realistic using every Steam metroidvania and 2D souls-like released from 2021 to October 2026: 1,623 games, flops included. About a nine-minute read.

What's inside:

1. **The lead idea:** how it plays, its moves and fights, heat, the map, the world and what to test first.
2. **What the market looks like:** how many games reach each review count (the median has 19) and how much price matters.
3. **What's crowded and what pays off:** which Steam tags are filling up, which ones change the odds of reaching 500 reviews, and a map of every game by tag similarity.
4. **How our ideas compare:** historical model estimates from uniform design evidence and expected tags, with fit uncertainty and stability checks.
5. **How we did it, and the limits.**
6. **The games:** a searchable table of all 1,623.

The deeper dive into the 250 most-reviewed metroidvanias, hand-scored on 148 design traits, lives in the [original research atlas](https://claude.ai/artifact/WZh1xcy9SyoqdqMCTFExo6).

## Contents

- `index.html`: the paper, self-contained (charts, data and images are embedded)
- `data/population_games.csv`: all 1,623 games with release date, all-language reviews, price band and top Steam tags
- `data/population_stats.json`: the original market and tag analysis (review ladder, price bands, tag effects, crowding and map)
- `data/stable_score.json`: the updated idea comparison, validation and stability results
- `data/stable_score_report.md`: the method, development history, limits and reproduction commands
- `data/stable_score_games.csv`: held-out predictions for all 1,245 games eligible for modelling
- `data/uniform_design_evidence.json`: literal feature evidence for each game and concept
- `data/games.csv` and `data/paper_stats.json`: the older top-250 data behind the atlas
- `assets/`: the diver sketch and the movement diagram

## Sources

Steam's store, search and review APIs. Outcomes and the market analysis are frozen at 16 October 2026; uniform store descriptions and up to 20 tags were collected on 18 October. The updated model includes all 153 hits and all 1,092 non-hits released at least a year before the snapshot. Every game and idea receives the same 300-character/seven-tag evidence budget, matching the seven main concept tag guesses. Extra real-game tags stay outside the model. Unsupported traits remain unknown.

Nested validation includes calibration, whole mixed-batch holdouts, split seeds, non-hit-deletion fits and 200 retuned bootstraps. Precise ranks and two-year launch-success claims are avoided. Built for ECE 194 with Python (scikit-learn, UMAP, joblib).

The candidate design view records supported advertised mechanics and structure. Inferred narrative and emotional judgments are excluded, and all feature effects require at least 25 training observations. The final selection assigns 0% to the design view, 60% to tags and 40% to the control-only baseline: the data did not establish an additional design-based success signal. Trait observations remain descriptive; the original full hand annotations are preserved in the atlas.
