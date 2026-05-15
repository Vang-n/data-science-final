---
layout: default
---

## Week 11 Update

### Data Source & Why:

- Personal match data exported from SwingVision, a tennis AI tracking app
- Each match exports as an Excel file with 5 sheets: shots, points, games, sets, stats
- Chose it because it's shot-level granular, personally meaningful, and has coordinate data (x/y) that enables spatial analysis
- Primary sheet is shots — one row per shot with player, stroke, spin, speed, placement, direction, and result

### Acquiring the Data:

- Exported each match individually from the SwingVision app as an Excel file
- Uploaded all files to a Google Drive folder
- Loaded and concatenated all 5 match files in Google Colab using pandas and glob
- Currently have 962 shots across 5 matches loaded into a master dataframe

### Strengths & Limitations:

- Strengths: shot-level granularity, x/y court coordinates, speed and spin on every shot, natural sequential structure enabling pattern analysis, opponent-specific breakdowns possible
- Limitations: only 5 matches exported so far, only captures my side reliably, no explicit point score state (need to reconstruct from points sheet), can't capture mental/physical context, sample sizes for specific situations may be small

### Preliminary Analysis Findings:

- Data loaded cleanly with no major missing values
- Two players per file — filtering to my name (Nana Vang) is required for all analysis
- Shot types, strokes, spin types, and directions are consistently labeled across matches
- x/y coordinate columns are populated and ready for heatmap visualization
- 962 shots across 5 matches gives enough data for clustering and win rate breakdowns

### Cleaning & Wrangling:

- Done: loaded all 5 files into master dataframe, added match_file tracking column, filtered to my shots only
- Still needed:
    - Extract match date from filename into its own column
    - Merge points sheet onto shots sheet to create a won_point column (this unlocks all win % analysis)
    - Normalize any inconsistent categorical values across match exports
    - Engineer a won_point flag (0/1) per shot based on point outcome

### Anticipated Challenges

- Merging points sheet back onto shots sheet to get point outcomes is the critical blocker — everything depends on this
- Sample sizes for specific shot combinations (e.g. wide serve on ad side in a break point) may be too small to draw conclusions
- K-means clustering will require feature normalization and choosing the right number of clusters (k) which needs research
- Sequential pattern analysis using shift() requires careful handling of rally boundaries so patterns don't bleed across points
