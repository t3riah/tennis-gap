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

## Infographics — Tennis, by the Numbers

**Live:** https://t3riah.github.io/tennis-gap/infographics/

Two versions together on one page, with a Simple / Pro switch:

- **Simple** (`infographics/simple.html`) — the plain-language explainer: the Rule of 100 (Hold % + Break %), court surfaces, the wind factor, live warning signs, and favorites vs. underdogs. Includes a working Rule of 100 calculator.
- **Pro** (`infographics/pro.html`) — what actually drives wins: SPW / RPW and their composite, the 6 serve-split numbers with separate ATP / WTA averages, the per-serve matchup model, and which popular stats are noise.

## Play — the interactive tool

**Live:** https://t3riah.github.io/tennis-gap/play/

One page, three tools, plain words first (exact numbers behind a toggle): **Explore a player** (her real serve stats on sliders — live hold and match strength vs. a tour-average opponent), **Compare a match** (what-if serve sliders on either player, plus the smallest single change that would flip the match), and **Follow live** (score steppers that give the exact win probability from the current score, set and game included). It runs on the same validated serve-model math and player data as the predictor.
