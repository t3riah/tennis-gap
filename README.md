# Tennis Gap — Player Dashboard

A free, no-signup, mobile-first dashboard for looking up tennis players and matchups. It is deliberately narrower than a general scores app: type one name for a player dashboard, or two names for a head-to-head.

**Live site:** https://t3riah.github.io/tennis-gap/

## What it does

- **Player dashboard** — hold and break rates, service/return points won, first- and second-serve splits, return splits, break-point save rate, per-match counting stats, and a by-surface breakdown, all beside tour averages. Each percentage also shows the player's tour rank in that category (among players with 10+ charted matches).
- **Head-to-head** — the same dashboard for two players, plus an exact serve-aware win probability (first serve, second serve, and double faults modeled separately), a likely range, the key matchup edges, matchup-specific serve numbers, per-surface win rates, and set-score probabilities under an expandable section.
- **Recent results** — each player's latest tour matches (event, round, opponent, score) from the results archive, with a freshness line at the top of the page stating exactly how current each data layer is.

Player lists are alphabetical and searchable by surname, full name, or the dropdown. Every player with at least one charted match is listed; very small samples are labelled as limited.

## Data

Profiles are built from the [Match Charting Project](https://github.com/JeffSackmann/tennis_MatchChartingProject), recency-weighted and shrunk toward tour averages so small samples don't shout. An all-surface profile appears once a player has one charted match; a surface-specific profile replaces it only after five charted matches on that surface. Recent results come from community archives of official tour records (ATP: ManTennisData; WTA: tennis-data.co.uk via the Wayback Machine). Both layers refresh automatically when their sources publish; the page always labels how fresh each layer is. Stats are informational only, not betting advice.

This repo contains only the static site. The full engine lives in a private repository.

## Infographics — Tennis, by the Numbers

**Live:** https://t3riah.github.io/tennis-gap/infographics/

Two versions together on one page, with a Simple / Pro switch:

- **Simple** (`infographics/simple.html`) — the plain-language explainer: the Rule of 100 (Hold % + Break %), court surfaces, the wind factor, live warning signs, and favorites vs. underdogs. Includes a working Rule of 100 calculator.
- **Pro** (`infographics/pro.html`) — what actually drives wins: SPW / RPW and their composite, the 6 serve-split numbers with separate ATP / WTA averages, the per-serve matchup model, and which popular stats are noise.

## Play link

The former slider-based Play page has been retired in favor of the single dashboard. https://t3riah.github.io/tennis-gap/play/ now redirects to the dashboard so older links keep working.
