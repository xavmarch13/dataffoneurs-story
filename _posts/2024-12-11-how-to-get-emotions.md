---
layout: post
title:  "Oppenheimer discovers sentiment analysis"
weight:  2
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/oppenheimer.jpg
previous_post: /dataffoneurs-story/mediator/feature/2024/12/11/Presentation-of-the-dataset.html
next_post: /dataffoneurs-story/data analysis/sentiment analysis/movies/2024/12/11/general-emotion.html
---




# Methodology: decoding movie emotions
<br>

In the quiet of his study, Oppenheimer pondered the intricate dance of human emotions within cinematic narratives. He envisioned a method to quantify these sentiments; to decode the emotional currents that drive storytelling. Understanding how emotions are embedded in films could give him the key to cinema.


As an engineer, Oppenheimer understood the necessity of pristine data. He meticulously cleansed the data, removing unfitting elements to reveal the essence of each narrative. To ensure the summaries were sufficiently comprehensive for meaningful analysis, Oppenheimer replaced shorter summaries with more detailed versions from Wikipedia when available. He then observed the length of summaries:

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/summary_length_distribution.html" width="100%" height="600" frameborder="0"></iframe>


Faced with the challenge of segmenting movie plots into time-series, Oppenheimer decided to first do a sentence-by-sentence sentiment analysis. The scientist decided to give its trust to a multi-class emotion classifier capable of discerning seven distinct emotions: anger, joy, surprise, disgust, sadness, fear, and neutrality. He has given us a proof of concept: 

<iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/sentences_with_dominant_emotions_highlighted.html" width="100%" height="600" frameborder="0"></iframe>

<br />

Oppenheimer was now faced with yet another problem. How was he going to be comparing time-series of such a variety of sizes ? Helped with the previously found median of 17 sentences per film. He concluded that evaluating movies in 20 points would be enough. Therefore he finally interpolated (or extrapolated when needed) all emotional arcs to fit 20 timesteps.

As a perfectionist, he also gave two different ways of visualizing his end results for a movie.

1. **True Emotional Data:** Raw output from sentiment analysis after interpolation.
    <iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/emotional_arc_of_the_movie.html" width="100%" height="600" frameborder="0"></iframe>
2. **Strongest Emotion Highlighted:** A visualization emphasizing the dominant emotion at each timestep.
    <iframe src="{{ site.baseurl }}/assets/plot/how_to_get_emotions/strongest_emotion_highlighted_across_timesteps.html" width="100%" height="600" frameborder="0"></iframe>

After all this research, Oppenheimer is tired. But are you ready to discover more? Let's follow Neo through the Matrix of emotions in movies.