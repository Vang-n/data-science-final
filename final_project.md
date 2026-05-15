---
layout: default
title: Final Project
---

# Tennis Match Analysis Project

## Overview

This project analyzes personal tennis match data collected through SwingVision in order to better understand patterns in serving, rally construction, positioning, and shot selection.

The goal of this project is to use data science techniques to identify what strategies contribute most to winning points and where improvements can be made.

---

# Serve Analysis

## First vs. Second Serve Performance

One of the first questions I wanted to explore was whether my first serve actually creates a measurable advantage compared to my second serve.

![Serve Results](images/serve_results.png)

The data shows that points beginning with a first serve are won at a significantly higher rate than points beginning with a second serve. This suggests that serve quality plays an important role in early point control.

---

# Serve Placement Heatmap

Another area I explored was serve location.

![Serve Heatmap](images/serve_heatmap.png)

This heatmap reveals that my most successful serves tend to pull opponents wide, especially on the deuce side. However, I noticed that I do not naturally target these areas as consistently as I expected.

---

# Rally Length Analysis

## Short vs. Long Rallies

I grouped rallies into categories based on shot count to better understand which point structures favor my game style.

![Rally Length Chart](images/rally_chart.png)

Interestingly, longer rallies produced higher win percentages than shorter points. This suggests that I become more successful once points become more neutral and extended.

---

# Net vs. Baseline

I also compared point outcomes when approaching the net versus staying at the baseline.

![Net vs Baseline](images/net_vs_baseline.png)

Although net approaches occurred less frequently, they resulted in a higher success rate overall. This may suggest that I should look for more opportunities to transition forward during matches.

---

# Challenges

One of the biggest challenges in this project was transforming raw match data into meaningful tennis concepts. Many tactical ideas in tennis are not directly labeled in the dataset, so I had to create my own definitions and categories.

For example:
- identifying drop shots
- grouping rally lengths
- interpreting serve placement coordinates
- distinguishing player labels between matches

Another challenge was balancing technical analysis with readability. I wanted the project to remain understandable even for readers without coding or tennis backgrounds.

---

# Conclusion

This project helped demonstrate how sports performance data can reveal patterns that are difficult to notice during actual competition. By combining tennis knowledge with data science techniques, I was able to identify both strengths and weaknesses in my own game while also learning new visualization and data analysis skills.
