---
layout: post
title:  "Do Longer Movies Tell More Emotional Stories? Exploring Emotional Complexity in Runtime"
weight:  5
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/xUtR9aTaqj4XTDDUgWwTrC.jpg
image2: /assets/images/xUtR9aTaqj4XTDDUgWwTrC.jpg
---

Movies have the power to evoke a spectrum of emotions, from joy and sadness to anger and surprise. But does the length of a movie influence how complex its emotional journey can be? In this analysis, Neo explores whether longer movies, with runtimes exceeding 2 hours, exhibit more intricate emotional arcs compared to their shorter counterparts. By analyzing emotional metrics derived from sentiment analysis, Neo investigates the relationship between runtime and emotional storytelling.

Neo, as usual, dives into the data with his characteristic curiosity, seeing the emotional journey of each movie as a code waiting to be cracked.

## Methodology: Measuring Emotional Complexity

<br />

### 1. Data Sources and Cleaning

Neo began by merging emotional data from sentiment analysis models with metadata about movie runtimes. The emotional data consisted of seven key emotions (anger, disgust, fear, joy, neutral, sadness, and surprise) extracted from movie plot summaries. Each emotional arc was standardized to 20 timesteps to ensure comparability between movies of varying plot lengths.

### 2. Calculating Emotional Metrics

To quantify emotional complexity, Neo computed three key metrics for each movie:

- **Amplitude:** The difference between the maximum and minimum emotion values.
- **Standard Deviation:** The variability of emotion intensity throughout the plot.
- **Sum of Absolute Changes:** The cumulative magnitude of emotion shifts between consecutive timesteps.

### 3. Categorizing Movies by Runtime

Neo then categorized movies into two groups based on their runtime:
- **Short Movies:** Runtimes ≤ 120 minutes.
- **Long Movies:** Runtimes > 120 minutes.

This classification allowed him to compare emotional complexity between the two groups.

## Results

### Emotional Complexity vs Runtime

When comparing emotional complexity metrics (amplitude, standard deviation, and sum of absolute changes) between short and long movies, Neo observed that:

- Long movies showed slightly higher variability in emotional arcs, but the differences were modest.
- Emotional complexity appeared to be influenced by factors beyond runtime, such as genre and storytelling style.

<iframe src="{{ site.baseurl }}/assets/plot/emotional_arcs_in_movies\mean_emotional_variation.png" width="100%" height="600" frameborder="0"></iframe>

These results were not enough for Neo to conclude that longer movies inherently have more variation in emotional arcs or a more complex storyline. He decided to dive deeper by analyzing each emotion individually.

### Correlation Analysis

Neo computed the correlation between runtime and emotional complexity metrics for each emotion:

<iframe src="{{ site.baseurl }}/assets\plot\emotional_arcs_in_movies\emotional_complexity_emotions.png" width="100%" height="600" frameborder="0"></iframe>

The correlation varied depending on the emotion considered. The highest correlation was for disgust, suggesting that as the movie length increases, the variation in this emotion also increases, leading to more emotional complexity. There were notable differences in correlation for emotions like anger, disgust, joy, and neutral, while fear, sadness, and surprise showed very low correlation between runtime and emotional variation.


The correlation was positive but weak (r ≈ 0.15), suggesting that while runtime contributes to emotional complexity, other narrative elements play significant roles.

Neo's analysis revealed that while longer movies tend to exhibit slightly more complex emotional arcs, runtime alone does not fully account for emotional storytelling.
Neo reflected on this, thinking about how a movie’s emotional depth cannot be reduced to just its runtime. There’s more to the emotional storytelling—something hidden in the layers of the plot, the pacing, and the way the characters evolve.

Stay tuned as Neo uncovers more insights into the emotional dynamics of cinematic storytelling!


