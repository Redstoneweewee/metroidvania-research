# The Metroidvania Gap

**Read the paper: https://redstoneweewee.github.io/metroidvania-research/**

An interactive research paper that maps the 250 most-reviewed metroidvanias in a 148-dimension design space, measures what travels with popularity, finds combinations nobody has built, and pitches **Thermocline**, a game designed for those gaps.

## Contents

- `index.html`: the paper, self-contained (charts, data and sketch are embedded)
- `data/games.csv`: all 250 games with every annotated design dimension
- `data/paper_stats.json`: cross-validated predictions, concept scores and bootstrap rank stability

## Sources

Steam store and review APIs and SteamSpy (accessed 16 October 2026); console sales from VGChartz, Nintendo and press reports. Built for ECE 184 with Python (scikit-learn, UMAP).
