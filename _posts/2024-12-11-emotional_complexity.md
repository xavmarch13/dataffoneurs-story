---
layout: post
title:  "Do Longer Movies Tell More Emotional Stories? Exploring Emotional Complexity in Runtime"
weight:  5
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/779-aurora-cinema.jpg
image2: /assets/images/779-aurora-cinema.jpg
---

Movies have the power to evoke a spectrum of emotions, from joy and sadness to anger and surprise. But does the length of a movie influence how complex its emotional journey can be? In this analysis, we explored whether longer movies, with runtimes exceeding 2 hours, exhibit more intricate emotional arcs compared to their shorter counterparts. By analyzing emotional metrics derived from sentiment analysis, we investigated the relationship between runtime and emotional storytelling.

## Methodology: Measuring Emotional Complexity

<br />

### 1. Data Sources and Cleaning

We began by combining emotional data from our sentiment analysis models with metadata about movie runtimes. The emotional data consisted of seven key emotions (anger, disgust, fear, joy, neutral, sadness, and surprise) extracted from movie plot summaries. Each emotional arc was standardized to 20 timesteps to ensure comparability between movies of varying plot lengths.

### 2. Calculating Emotional Metrics

To quantify emotional complexity, we computed three key metrics for each movie:

- **Amplitude:** The difference between the maximum and minimum emotion values.
- **Standard Deviation:** The variability of emotion intensity throughout the plot.
- **Sum of Absolute Changes:** The cumulative magnitude of emotion shifts between consecutive timesteps.

### 3. Categorizing Movies by Runtime

We categorized movies into two groups based on their runtime:
- **Short Movies:** Runtimes ≤ 120 minutes.
- **Long Movies:** Runtimes > 120 minutes.

This classification allowed us to compare emotional complexity between the two groups.

## Results

### Emotional Complexity vs Runtime

When comparing emotional complexity metrics (amplitude, standard deviation, and sum of absolute changes) between short and long movies, we observed that:

- Long movies showed slightly higher variability in emotional arcs, but the differences were modest.
- Emotional complexity appeared to be influenced by factors beyond runtime, such as genre and storytelling style.

<iframe src="{{ site.baseurl }}/assets/plot/emotional_arcs_in_movies\mean_emotional_variation.png" width="100%" height="600" frameborder="0"></iframe>

These results are not enough to say if longer movies have more variations in their emotional arcs and more complex storyline. We can further our analysis by looking at each emotion individually

### Correlation Analysis

We computed the correlation between runtime and emotional complexity metrics for each emotion:

<iframe src="{{ site.baseurl }}/assets\plot\emotional_arcs_in_movies\emotional_complexity_emotions.png" width="100%" height="600" frameborder="0"></iframe>

The correlation varies a lot depending on which emotion is considered. The highest correlation is for disgust, suggesting that as the movie get longer, the variation in this emotion is stronger, leading to more emotional complexity in the film. We can note large difference depending on the emotion anger, disgust, joy and neutral while fear, sadness and surprise have very low correlation between movie runtime and emotional variation. 

(For all emotion mais à voir si ca dégage)
The correlation was positive but weak (r ≈ 0.15), suggesting that while runtime contributes to emotional complexity, other narrative elements play significant roles.

Our analysis revealed that while longer movies tend to exhibit slightly more complex emotional arcs, runtime alone does not fully account for emotional storytelling.

Stay tuned as we uncover more insights into the emotional dynamics of cinematic storytelling!
