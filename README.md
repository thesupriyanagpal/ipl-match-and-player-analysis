# IPL Match and Player Performance Analysis (2008–2019)

**IPL Matchroom** is an interactive dashboard built from 756 Indian Premier League matches across 12 seasons. It explores franchise performance, toss decisions, run chases, and player records using historical match and ball-by-ball data.

## Problem Statement

Which franchises won most consistently? How often did teams chase successfully at different first-innings totals? Which players stood out for batting volume, scoring speed, or wickets?

Franchises played different numbers of matches, and batters faced different numbers of deliveries. The dashboard shows counts alongside rates and denominators, so readers can compare performance with that context in view.

## Dashboard Features

| View | What you can explore |
| --- | --- |
| Franchise performance | Compare wins and win rates, or use the season-by-season heatmap to see how each franchise performed over time. |
| Toss decisions | Track how often toss winners chose to field first across seasons. |
| Scoring and chasing | Explore the distribution of first-innings totals, chase success by score band, and the split between wins batting first and chasing. |
| Player performance | Switch between batting runs, credited wickets, and Player of the Match awards. Adjust the minimum deliveries faced in the batting scatter plot and compare four-run and six-run events among leading batters. |

The season filter applies to both match and player views. The franchise filter applies to match views. When a franchise is selected, opponent records reflect only games against that franchise.

## Key Findings

- **Mumbai Indians recorded the most wins (109).** Chennai Super Kings had the highest win rate (61.0%) among franchises with at least 50 decided appearances.
- **Toss winners won 393 of 752 decided matches (52.3%).** This describes the historical record. It does not establish a causal toss advantage.
- **Chase success was lower in the higher scoring band.** Among eligible matches that passed the score consistency check, chasing teams won 72.7% of matches with first-innings scores of 120–149 runs, compared with 36.7% for scores of 180–209 runs.

## Data and Methodology

- Standardized dates and franchise aliases, preserved match IDs, and removed 23 exact duplicate delivery records within the same match. Kept records with repeated ball labels when their details differed.
- Calculated win rates using decided appearances, including ties with a recorded winner.
- Excluded ties, no-results, rain-adjusted matches, and 30 ordinary matches that failed a score consistency check from the chase analysis.
- Used non-wide delivery records as a proxy for balls faced in the batting scatter plot.

The archive ends in 2019. Team, venue, weather, and season differences can affect the comparisons.

[Source data and reference notebook](https://github.com/iyanagpal/Exploratory-Data-Analysis-Sports/tree/d9bf3bfdf64c9f5da3da83cd5eb8a0a35246ddb8)


## Repository Structure

| File | Purpose |
| --- | --- |
| `ipl/index.html` | Dashboard layout and methodology notes |
| `ipl/style.css` | Styling and responsive layout |
| `ipl/app.js` | Filters, charts, and interactive summaries |
| `ipl/data.js` | Prepared IPL data used by the dashboard |

## Author

**Dr. Supriya Nagpal** · [Portfolio](https://thesupriyanagpal.com/)
