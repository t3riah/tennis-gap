# Tennis Gap — Player Stats & Match Predictor

A free, no-signup web tool for browsing real tennis stats and predicting matches.

**Live site:** https://t3riah.github.io/tennis-gap/

## What it does

- **Player Stats** — compare any two ATP or WTA players: service points won, return points won, hold and break rates, first/second serve splits, break-point save rates, and recent-form freshness for each player.
- **Match Predictor** — an exact serve-aware probability model (first serve, second serve, and double faults modeled separately) with a confidence range, the key matchup edge explained in plain language, exact set-score probabilities, and a per-surface breakdown.

Player lists can be browsed alphabetically or sorted by any stat — best servers, best returners, fewest double faults — per surface.

## Data

Profiles are built from the [Match Charting Project](https://github.com/JeffSackmann/tennis_MatchChartingProject), recency-weighted and shrunk toward tour averages so small samples don't shout. Stats are informational only, not betting advice.

This repo contains only the static site. The full engine lives in a private repository.
