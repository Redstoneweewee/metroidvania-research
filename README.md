# Metroidvania Research

**Read the paper: https://redstoneweewee.github.io/metroidvania-research/**

A short research brief for a student team. It pitches a **deep-sea heat metroidvania** (a platformer with gravity flipped: you float up, and going deeper means using the terrain), then checks what's realistic using every Steam metroidvania and 2D souls-like released from 2021 to October 2026: 1,623 games, flops included. About a nine-minute read.

What's inside:

1. **The lead idea:** how it plays, its moves and fights, heat, the map, the world and what to test first.
2. **What the market looks like:** how many games reach each review count (the median has 19) and how much price matters.
3. **What's crowded and what pays off:** which Steam tags are filling up, which ones change the odds of reaching 500 reviews, and a map of every game by tag similarity.
4. **How our ideas compare:** each idea's chance of reaching 500 reviews, from the tags we expect it to get.
5. **How we did it, and the limits.**
6. **The games:** a searchable table of all 1,623.

The deeper dive into the 250 most-reviewed metroidvanias, hand-scored on 148 design traits, lives in the [original research atlas](https://claude.ai/artifact/WZh1xcy9SyoqdqMCTFExo6).

## Contents

- `index.html`: the paper, self-contained (charts, data and images are embedded)
- `data/population_games.csv`: all 1,623 games with release date, all-language reviews, price band and top Steam tags
- `data/population_stats.json`: everything the paper's charts use (review ladder, price bands, tag effects, crowding, idea odds)
- `data/games.csv` and `data/paper_stats.json`: the older top-250 data behind the atlas
- `assets/`: the diver sketch and the movement diagram

## Sources

Steam's store, search and review APIs, collected 16 October 2026. Built for ECE 194 with Python (scikit-learn, UMAP).
