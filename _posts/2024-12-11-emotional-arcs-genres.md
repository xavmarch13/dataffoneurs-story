---
layout: post
title:  "Emotional Arcs in Movies: A Universal or Genre-Specific Trend?"
weight:  4
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/movies-genres-that-defined-era-then-died-out.avif
image2: /assets/images/movies-genres-that-defined-era-then-died-out.avif
---

Emotions are the backbone of cinematic storytelling, captivating audiences and leaving lasting impressions. But do these emotional arcs follow universal patterns, or are they tailored to fit specific genres? In this post, we dive into emotional trajectories across different movie genres, using sentiment analysis to uncover whether genre dictates the emotional journey of a film.

Neo, the legendary hacker from The Matrix, finds himself reflecting on this question while navigating through streams of data. The question resonates with him deeply. After all, isn’t every journey—a story? Whether it’s dodging bullets or defying fate, Neo knows better than most that patterns are everywhere, even in the emotions that drive our stories forward.

Neo peers at the data flowing past him, an ocean of emotional peaks and valleys. To uncover meaning, he realizes, the system must be broken down into its parts—categorizing genres, tracing patterns, and finding anomalies.

Neo delves into the Matrix of Emotions to uncover the answers, guiding us through the data analysis that reveals how emotions shift across cinematic genres.

## Methodology: Analyzing Genre-Specific Emotional Patterns

<br />

### 1. Data Collection and Categorization

Neo used movie summaries from the CMU Movie Summary Corpus and was provided with additional data scraped from Wikipedia. Each movie was tagged with its primary genre(s), enabling Neo to group emotional arcs by genre for comparative analysis. 

Because of the astronomic number of genres in the data (about 360), Neo decided to handcraft a mapping to go down from 300 plus genres of movies to about a dozen. While Neo's mapping may be a point of discussion among movie enthousiasts, Neo find it a good approximation to a more general genre classification. 

Neo pauses. “Reduction,” he murmurs. “Finding simplicity in the noise. It’s like filtering out the static in the Matrix.”

### 2. Genre distribution
Neo first take a look at the genres distribution in films.
<iframe src="{{ site.baseurl }}/assets/plot\emotional_arcs_genres\distribution_movie_genres.png" width="84%" height="500" frameborder="0"></iframe>
Drama is the most common genre, accounting for the largest proportion at approximately 26%. This is followed by comedy and thriller, which hold significant but smaller shares. The distribution suggests a diverse set of genres without a single dominant category, reflecting the varied preferences in cinematic storytelling. 

Neo smirks. “Drama. Of course. Conflict defines us, doesn’t it? The choices we make, the consequences we endure. But diversity in stories… that’s the humanity behind it all.”

### 4. Visualizing Emotional Arcs by Genre

To visualize emotional trajectories, Neo plotted the normalized emotional arcs for each genre over 20 timesteps. 

<iframe src="{{ site.baseurl }}/assets/plots_alix\continentvsgenres.html" width="100%" height="600" frameborder="0"></iframe>


### The Consistent Rhythm of Emotional Arcs Across Genres    

### Universal vs. Genre-Specific Emotional Patterns  
Neo identifies three emotions—anger, joy, and disgust—that seem to transcend genre boundaries.

Neo's analysis reveals that some emotions, such as anger, joy, and disgust, follow very similar trajectories regardless of the genre. In contrast, emotions like fear, sadness, and surprise show significant variability depending on the type of story being told.

Joy usually starts high, then drops as we move further in the story, only to rise back up at the end, reflecting resoltuion

But Neo, ever the questioner, probes further. Why do some genres, like Horror or Romance, deviate from this structure? The answer lies in how emotions function within different storytelling frameworks and this distinction can be understood by examining the **storytelling conventions** and the **inherent characteristics** of these emotions. 

This universal structure suggests that filmmakers rely on common narrative techniques to captivate audiences across different genres.  

### **1. The Universal Role of Joy, Anger, and Disgust**  

- **Joy and Anger as Narrative Pillars:**  

Neo realizes that filmmakers use emotions strategically to meet audience expectations:

Joy and anger are universal emotions that frequently shape the core of cinematic storytelling. **Joy** usually starts high, then drops as we move further in the story, only to rise back up at the end, reflecting resolution, triumph, or humor, while **anger** starts low only to rise during the movie, to finally drops back down at the end, reflecting that anger grows during moments of conflict, betrayal, or injustice in the middle of the movie, and drop at the end when there's triumph, resolution or humor. These elements are staples of nearly every genre, ensuring that joy and anger arcs remain largely consistent across diverse narratives. These emotions mirror Neo’s journey through struggle, revelation, and triumph.

- **Disgust’s Steady Arc Across Genres:**  
  Unlike more dynamic emotions, **disgust** tends to play a subtler, secondary role in storytelling. Disgust generally follows an emotional arcs that grows in the middle of the movie, showing disgust as conflict and challenges arises in the middle of the movie. It often manifests in reaction to specific events—such as repugnant behavior or unsettling scenarios—rather than driving the story forward. It then falls off in the second half of the movie to finally have practically no disguts. This situational nature results in a stable arc for disgust across genres, with minimal variations  

- **Narrative Archetypes and Consistency:**  
  Across genres, many stories follow shared archetypes, such as the "hero's journey," which naturally incorporates anger, disgust, and joy. These emotions mark key stages in the narrative: anger during challenges, disgust when confronting unpleasant truths, and joy at the resolution of the conflict. Their consistent presence underscores their foundational role in storytelling.  

### **3. Emotional Functions in Storytelling**  

- **Primary vs. Contextual Emotions:**  
  Neo finds that motions like anger, joy, and disgust serve as "primary emotions", essential for driving the plot and defining key narrative moments. On the other hand, fear, sadness, and surprise act as "contextual emotions," their intensity and role dictated by the genre’s tone and purpose.  

- **Meeting Audience Expectations:**  
  Audience expectations also play a significant role in shaping emotional arcs. For example, Horror audiences anticipate fear and surprise, while Drama viewers expect a mix of sadness and joy. **Disgust**, meanwhile, serves as a versatile tool across genres, punctuating specific scenes without dominating the narrative.  

### **Conclusion**  

Much like Neo’s journey, the emotional arcs of movies reflect both universal truths and unique challenges. The universality of emotions like anger, joy, and disgust reflects their foundational role in storytelling, while the variability of emotions like fear, sadness, and surprise highlights the creative flexibility filmmakers employ to craft genre-specific narratives.

As Neo steps out of the Matrix, he leaves us with a thought:

“Storytelling is about choice—whether it’s the red pill or the blue, or how we shape emotions to tell tales that resonate. What’s your choice?”


