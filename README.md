# Guilford County Neighborhood Vitality Index (GCNVI)

A block-group-level measure of neighborhood conditions for all 338 block groups of Guilford County, North Carolina: 220 verified variables, distilled by criterion validation to ten transparent components, validated against the Opportunity Atlas mobility outcomes and the Child Opportunity Index 3.0 (r = .62 to .87), and classified into five vitality categories.

**Sponsored by Jeff Thigpen, Guilford County Register of Deeds, and Shaunne Thomas, Director, Guilford County Small Business Entrepreneurship Department**, in support of the Guilford County Community Data Atlas and the Coalition of Anchors.

## Interactive map

The repository's GitHub Pages site serves an interactive map of the index: the composite score and five-category classification, with switchable layers for each of the ten components, red-to-green with green always the direction of greater vitality, priority tracts outlined, and a full block-group profile on click.

Once Pages is enabled (Settings > Pages > deploy from branch, root), the map is at: `https://<username>.github.io/<repo-name>/`

## Documents

| Document | File |
|---|---|
| Final report (2026) | [docs/GCNVI_Final_Report_2026.pdf](docs/GCNVI_Final_Report_2026.pdf) |
| Atlas of Neighborhood Conditions (213 plates + index) | [docs/IRI_Guilford_County_Neighborhood_Atlas_2026.pdf](docs/IRI_Guilford_County_Neighborhood_Atlas_2026.pdf) |
| Concentrated Disadvantage and the Geography of Opportunity (framing) | [docs/Concentrated_Disadvantage_Framing_2026.pdf](docs/Concentrated_Disadvantage_Framing_2026.pdf) |
| Neighborhood Indicators and Indices: Literature Review | [docs/Neighborhood_Indicators_LitReview_2026.pdf](docs/Neighborhood_Indicators_LitReview_2026.pdf) |
| GCNVI Methodology | [docs/GCNVI_Methodology_2026.pdf](docs/GCNVI_Methodology_2026.pdf) |

## Data

- `data/GCNVI_v1_Scored_Dataset.csv` — one row per block group: GEOID, ten vitality-aligned component z-scores, composite score, five-category classification.
- `data/gcnvi_blockgroups.geojson` — simplified 2020 block-group geometry with scores, categories, and raw component values (the map's data layer).
- `data/layers.json` — layer metadata (labels, polarity, display ranges).

**Notes for data users.** Scores are county-relative (z within Guilford County) and support no cross-county comparison. Suppressed cells (small-count birth outcomes; state-suppressed life-expectancy tracts) are carried as empty, never imputed. The personal-crime component is a modeled vendor index cleared for the accompanying analyses; its license governs any further republication. Demographic composition is excluded from all scoring by design: the index measures the conditions of places, never the worth of people.

## Citation

Sills, S. J. (2026). *The Guilford County Neighborhood Vitality Index: Final report.* Winston-Salem, NC: Innovative Research Insights, LLC.

© 2026 Innovative Research Insights, LLC. Documents and data are provided for public-interest use with attribution.
