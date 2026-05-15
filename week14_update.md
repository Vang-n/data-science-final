---
layout: default
title: Week 14 Update
---

# Week 14 Update

### Project Progress

At this point, I have made a lot of progress on the project and have completed most of the main analysis sections. The notebook now includes work on serves, rally length, positioning, drop shots, and backhand slice patterns. I also have a few visualizations finished.

What is left now is working out all of the visuals as well as writing the reflections and adding the narrative aspect through the project to make it organized and easier to follow.

### New Technique I Researched

One new technique I had to learn for this project was how to build more advanced visualizations and sequence-based analysis from match data. In particular, I had to figure out how to work with heat maps, interactive Plotly charts, and multi-shot sequence tracking.

This was not something I was already comfortable doing at the start of the project, so I learned by experimenting in Google Colab, looking at examples online, and using the structure of my own dataset to guide how I built the analysis. I also learned how to use pandas tools like `pd.cut()` to group rally lengths into categories, which helped turn the raw point data into something more readable.

### Communication Strategy

For the final project, I want to present the analysis in a way that starts broad and then becomes more specific. I think the best structure is to begin with serving and overall point patterns, then move into court positioning and rally length, and finish with the more specific tactical shots like drop shots and backhand slices.

I plan to use the project webpage itself as the main presentation format, since it allows the visualizations and written explanation to stay together.

### Challenges and Reflection

One of the biggest challenges in this project has been working with real match data that is messy and not always labeled in the most convenient way. A lot of the work was not just analysis, but figuring out what the data actually meant and how to turn it into categories that made sense for tennis.

For example, there is no direct "drop shot" column, so I had to define one myself based on bounce location, spin, and speed. I also had to think carefully about how to interpret shot locations and player labels so the analysis stayed accurate. Another difficult part was building the heat map, since getting the coordinates to line up correctly with the service boxes took a lot of trial and error.

Even though those parts were frustrating at times, they ended up being some of the most useful parts of the project because they forced me to think more carefully about both the tennis and the coding.
