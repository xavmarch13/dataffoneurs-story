---
layout: post
title:  "Emotional Arcs in Movies: A Universal or Genre-Specific Trend?"
weight:  2
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/movies-genres-that-defined-era-then-died-out.avif
image2: /assets/images/movies-genres-that-defined-era-then-died-out.avif
---

## Introduction

Emotions are the backbone of cinematic storytelling, captivating audiences and leaving lasting impressions. But do these emotional arcs follow universal patterns, or are they tailored to fit specific genres? In this post, we dive into emotional trajectories across different movie genres, using sentiment analysis to uncover whether genre dictates the emotional journey of a film.

## Methodology: Analyzing Genre-Specific Emotional Patterns

<br />

### 1. Data Collection and Categorization

We used movie summaries from the CMU Movie Summary Corpus and supplemented them with additional data scraped from Wikipedia. Each movie was tagged with its primary genre(s), enabling us to group emotional arcs by genre for comparative analysis. 

Because of the astronomic number of genres in the data (about 360), we decided to handcraft a mapping to go down from 300 plus genres of movies to about a dozen. While our mapping may be a point of discussion among movie enthousiasts, we find it a good approximation to a more general genre classification. 

### 2. Genre distribution
We can first take a look at the genres distribution in films.
<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\distribution_movie_genres.png" width="100%" height="600" frameborder="0"></iframe>
Drama is the most common genre, accounting for the largest proportion at approximately 26%. This is followed by comedy and thriller, which hold significant but smaller shares. The distribution suggests a diverse set of genres without a single dominant category, reflecting the varied preferences in cinematic storytelling. 

### 4. Visualizing Emotional Arcs by Genre

To visualize emotional trajectories, we plotted the normalized emotional arcs for each genre over 20 timesteps. 

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Anger_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Disgust_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Fear_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Joy_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Neutral_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Surprise_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\Normalized_Evolution_of_Sadness_across_Timesteps_for_Each_Genre.png" width="100%" height="600" frameborder="0"></iframe>

### The Consistent Rhythm of Emotional Arcs Across Genres  

No matter the genre, emotional arcs in movies tend to follow a consistent pattern. Negative emotions like anger, fear, and disgust typically rise during the first half of a film, creating tension, while neutrality and joy gradually increase towards the conclusion, providing emotional resolution. This universal structure suggests that filmmakers rely on common narrative techniques to captivate audiences across different genres.  

### Universal vs. Genre-Specific Emotional Patterns  

Our analysis reveals that some emotions, such as anger, joy, and disgust, tend to follow similar trajectories regardless of the genre. In contrast, emotions like fear, sadness, and surprise show significant variability depending on the type of story being told.  

This distinction can be understood by examining the **storytelling conventions** and the **inherent characteristics** of these emotions.  

### **1. The Universal Role of Joy, Anger, and Disgust**  

- **Joy and Anger as Narrative Pillars:**  
  Joy and anger are universal emotions that frequently shape the core of cinematic storytelling. **Joy** reflects resolution, triumph, or humor, while **anger** often arises during moments of conflict, betrayal, or injustice. These elements are staples of nearly every genre, ensuring that joy and anger arcs remain largely consistent across diverse narratives.  

- **Disgust’s Steady Arc Across Genres:**  
  Unlike more dynamic emotions, **disgust** tends to play a subtler, secondary role in storytelling. It often manifests in reaction to specific events—such as repugnant behavior or unsettling scenarios—rather than driving the story forward. This situational nature results in a stable arc for disgust across genres, with minimal variations in intensity or frequency.  

- **Narrative Archetypes and Consistency:**  
  Across genres, many stories follow shared archetypes, such as the "hero's journey," which naturally incorporates anger, disgust, and joy. These emotions mark key stages in the narrative: anger during challenges, disgust when confronting unpleasant truths, and joy at the resolution of the conflict. Their consistent presence underscores their foundational role in storytelling.  

### **2. Genre-Specific Nature of Fear, Sadness, and Surprise**  

- **Fear:**  
  As the cornerstone of Horror, **fear** plays a central role in evoking suspense and dread. It is nearly absent in lighthearted genres like Comedy or Romance, leading to wide variability in its prominence and trajectory across genres.  

- **Sadness:**  
  A defining feature of Drama and Romance, **sadness** adds emotional depth by exploring themes of loss, reconciliation, or personal growth. In contrast, genres like Action or Horror typically use sadness sparingly, focusing more on fast-paced tension or adrenaline.  

- **Surprise:**  
  Genres such as Horror and Sci-Fi thrive on **surprise**, leveraging twists and unexpected turns to keep audiences engaged. In contrast, Drama and Romance rely more on gradual emotional development, making surprise less integral to their storytelling.  

### **3. Emotional Functions in Storytelling**  

- **Primary vs. Contextual Emotions:**  
  Emotions like anger, joy, and disgust serve as "primary emotions," essential for driving the plot and defining key narrative moments. On the other hand, fear, sadness, and surprise act as "contextual emotions," their intensity and role dictated by the genre’s tone and purpose.  

- **Meeting Audience Expectations:**  
  Audience expectations also play a significant role in shaping emotional arcs. For example, Horror audiences anticipate fear and surprise, while Drama viewers expect a mix of sadness and joy. **Disgust**, meanwhile, serves as a versatile tool across genres, punctuating specific scenes without dominating the narrative.  

### **Conclusion**  

The universality of emotions like anger, joy, and disgust reflects their foundational role in storytelling, while the variability of emotions like fear, sadness, and surprise highlights the creative flexibility filmmakers employ to craft genre-specific narratives.