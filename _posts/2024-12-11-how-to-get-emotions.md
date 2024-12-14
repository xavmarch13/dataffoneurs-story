---
layout: post
title:  "Mapping Movie Emotions: Sentiment Analysis in Film Summaries"
weight:  2
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/movie_theatre.jpg
image2: /assets/images/movie_theatre.jpg
---

## Introduction

Movies are a universal language, capable of evoking powerful emotions that resonate with audiences across cultures and generations. Understanding how emotions are embedded in films can offer insights into their storytelling success, audience impact, and even their box office performance. To explore this, we embarked on a sentiment analysis journey by analyzing the text of movie summaries. This post outlines our methodology for mapping emotional dynamics in movies and highlights some of the fascinating insights we've uncovered.

## Methodology: Decoding Movie Emotions

<br />

### 1. Data Preparation and Cleaning

The foundation of any data analysis project is clean, reliable data. We started by compiling movie summaries from the CMU Movie Summary Corpus and supplemented missing or incomplete data with summaries scraped from Wikipedia. Each summary underwent a rigorous cleaning process to remove noise, including stripping HTML tags and odd citations, standardizing formatting inconsistencies and removing irrelevant metadata or redundant content.

To ensure the summaries were comprehensive enough for meaningful analysis, shorter summaries were replaced with longer versions when available. Below is a graph showcasing the distribution of summary lengths, revealing a highly skewed distribution with notable outliers:

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/summary_length_distribution.html" width="100%" height="600" frameborder="0"></iframe>

The left-skewed distribution posed a challenge since sentiment analysis relies on consistent time series data. To address this, we standardized the summaries by interpolating all time series data to 20 timesteps. This choice was guided by the median sentence count of 17 in movie summaries, providing a balanced compromise.

### 2. Segmenting Summaries

Initially, we aimed to segment movie plots based on sentence similarity using cosine similarity. However, even with low thresholds, this approach resulted in too few segments, making it unsuitable for time-series analysis. Given the median of 17 sentences per summary, we pivoted to a sentence-by-sentence sentiment analysis approach.

For sentiment analysis, we experimented with two models:

- A binary positive/negative sentiment classifier.
- A multi-class emotion classifier capable of detecting seven emotions: anger, joy, surprise, disgust, sadness, fear, and neutral sentiment.

The latter model was more informative and aligned with our goal of mapping emotional dynamics across movie plots.

### 3. Sentiment Analysis

The backbone of our sentiment analysis is a fine-tuned RoBERTa model trained on six diverse English datasets, including:

- **Crowdflower (2016):** Social media emotion annotations.
- **Emotion Dataset:** Curated for general-purpose sentiment analysis.
- **GoEmotions (Demszky et al., 2020):** Extensive emotion annotations for Reddit comments.
- **ISEAR (Vikash, 2018):** Emotion annotations in human interactions.
- **MELD (Poria et al., 2019):** Multimodal sentiment analysis in dialogue contexts.
- **SemEval-2018 (EI-reg):** Emotion intensity recognition.

This robust training foundation enables the model to output probability scores (ranging from 0 to 1) for each emotion. Below is an example visualization highlighting the dominant emotion sentence by sentence in a movie plot summary:

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/sentences_with_dominant_emotions_highlighted.html" width="100%" height="600" frameborder="0"></iframe>

<br />

### 4. Interpolating Emotional Arcs

To standardize the varying lengths of movie summaries, we interpolated all emotional arcs to fit 20 timesteps. This process ensured consistency across analyses, enabling direct comparisons between films. The interpolation was applied independently to each emotion, creating smooth, uniform time series data.

Below are three visualizations demonstrating this process:

1. **True Emotional Data:** Raw output from sentiment analysis after interpolation.
2. **Fitted Emotional Arc:** Fit of a smooth function om each emotion arc.
3. **Strongest Emotion Highlighted:** A visualization emphasizing the dominant emotion at each timestep.

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/emotional_arc_of_the_movie.html" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/fitted_emotional_arc_of_the_movie.html" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/strongest_emotion_highlighted_across_timesteps.html" width="100%" height="600" frameborder="0"></iframe>

## Conclusion

By dissecting movie summaries through sentiment analysis, we have begun to unravel the intricate emotional arcs that define storytelling in film. Our methodology; from data cleaning and interpolation to leveraging cutting-edge models; has enabled us to explore how emotions shape cinematic narratives across genres and time periods. Stay tuned as we dive deeper into these insights, examining correlations how emotions shape movies.
