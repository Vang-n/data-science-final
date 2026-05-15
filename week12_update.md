## Week 12 Update

### Exploratory Analysis & Visualizations

This week I focused on better understanding the dataset and starting to turn the raw match data into something more useful. The biggest step was beginning to explore patterns in my serves, rally lengths, and general point outcomes. Since this project is built around real match data, a lot of the early work has been about figuring out how the data is structured and what columns are actually useful for tennis analysis.

One challenge I ran into was making sure I was interpreting the SwingVision data correctly. Because the app labels players as "host" or "guest" depending on the match, I had to be careful about how I identified my own shots and point results. Once that was sorted out, I was able to start building cleaner visualizations and looking at the data more meaningfully.

So far, I have been exploring things like:
- serve direction and serve location
- first serve vs. second serve results
- rally length categories
- baseline vs. net performance

This week also gave me a chance to experiment with interactive Plotly visualizations. That was useful because it made the charts feel more readable and easier to explore, especially for serve placement and other shot-based patterns.

### Early Findings

Some early patterns are already starting to show up. For example, my longer rallies seem to be more successful than my shorter ones, which suggests I am more comfortable once a point becomes more neutral or extended. At the same time, a lot of my shorter points are not being won as consistently as I would like, which makes serve quality and early point construction even more important.

Another thing I noticed is that my serve placement does matter, but not always in the way I expect. I tend to get my best results when I move my opponent wide, even though my heatmap shows that I do not always naturally serve there as often as I should.

### Challenges

The main challenge this week was cleaning and organizing the data well enough to make the exploratory analysis useful. I also had to spend time figuring out how to make the visualizations match the tennis ideas I actually care about. For example, some of the categories in the raw data do not directly match the way a player thinks about tennis, so I had to create my own groupings and definitions to make the analysis more meaningful.
