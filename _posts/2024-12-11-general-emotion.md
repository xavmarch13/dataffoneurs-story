---
layout: post
title:  "2. Neo's Journey Through Emotion: Uncovering Patterns in Film Sentiment"
weight:  3
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/xUtR9aTaqj4XTDDUgWwTrC.jpg
image2: /assets/images/xUtR9aTaqj4XTDDUgWwTrC.jpg
previous_post: /dataffoneurs-story/data analysis/sentiment analysis/movies/2024/12/11/how-to-get-emotions.html
next_post: /dataffoneurs-story/jekyll/update/2024/12/12/sound-color-cinema.html
---

# The emotional journey

Emotions are the backbone of cinematic storytelling, captivating audiences and leaving lasting impressions. But do these emotional arcs follow universal patterns, or are they tailored to fit specific genres? In this post, we dive into emotional trajectories across different movie genres, using sentiment analysis to uncover whether genre dictates the emotional journey of a film.

Neo, the legendary hacker from The Matrix, finds himself reflecting on this question while navigating through streams of data. The question resonates with him deeply. After all, isn’t every journey—a story? Whether it’s dodging bullets or defying fate, Neo knows better than most that patterns are everywhere, even in the emotions that drive our stories forward.

Neo peers at the data flowing past him, an ocean of emotional peaks and valleys. To uncover meaning, he realizes, the system must be broken down into its parts—categorizing genres, tracing patterns, and finding anomalies.

Neo delves into the Matrix of Emotions to uncover the answers, guiding us through the data analysis that reveals how emotions shift across cinematic genres.

# Global emotional trends

### Average analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/average_emotion_intensity_across_movies.html" width="84%" height="500" frameborder="0"></iframe>
Peering at the boxplot data, Neo begins his analysis:

#### Neo’s Observations:
1. *Neutral Dominates*:  
   Neo notices that the neutral emotion reigns supreme, showing the highest overall intensity. Its broad range and numerous outliers reveal that neutral sentiment is globally prevalent, acting as a baseline or anchor emotion in many stories. “It’s the calm before the storm,” Neo mutters, recognizing how neutrality often serves as the foundation from which other emotions emerge.

2. *Sadness and Joy Stand Out*:  
   As Neo traces the distributions of sadness and joy, he notes their similar ranges. Sadness, however, has a slightly broader spread and more pronounced outliers. “Sadness... the weight of loss,” Neo reflects, recognizing its frequent, varied presence in narratives. Joy, on the other hand, represents moments of triumph, its distribution slightly narrower but still impactful. Together, these emotions mirror the rise and fall of human experience.

3. *Anger, Disgust, Fear, and Surprise Are Less Prominent*:  
   Neo points out that these four emotions have lower intensities compared to neutral and sadness. Anger, however, stands apart with a wider range. “Anger spikes,” Neo notes, “but it rarely lingers—it’s sharp, fleeting, and focused.” Surprise, meanwhile, has the smallest range, its bursts brief but meaningful, like the unexpected twists in the Matrix itself.

As Neo steps back, the patterns become clear. Each box in the plot represents a world of emotion—some dominant, others fleeting. Neutral anchors the journey, sadness gives it depth, joy offers relief, and anger, disgust, fear, and surprise provide sharp contrasts.

### Time-series analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/normalised_emotions_time_analysis.html
" width="84%" height="500" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

#### Neo's Observations:
1. *Initial Spike and Divergence*:
   - *Anger* starts with the lowest normalized intensity, then gradually rises during the story. Towards the end, anger experiences a significant decline.  
     *Interpretation*: Anger’s gradual rise and decline suggest it plays a role in building tension throughout the narrative, but it often resolves or diminishes by the conclusion.

   - *Joy* follows an inverse emotional arc, starting with a high normalized intensity, only to decline in the middle of the movie, and then rising back up towards the end.  
     *Interpretation*: Joy’s trajectory reflects uplifting beginnings and endings, bookending stories with hope or positivity despite darker or challenging middle arcs.

   - *Sadness* is high at the start of the story but declines quickly right after. In the middle of the story, *sadness* steadily increases throughout the timeline, becoming significant toward the later timesteps, before dropping back down at the end of the story.  
     *Interpretation*: Sadness appears to underpin pivotal emotional moments in the story, particularly in climaxes or resolutions, before giving way to a more uplifting or neutral conclusion.

   - Emotions like *fear* and *disgust* show similarities in their emotional arcs, both starting with high normalized intensity. Although *fear* remains quite constant during the story, unlike *disgust*, which starts declining early, they both end up with very low normalized intensity near the end due to a drop near the story's conclusion.  
     *Interpretation*: Fear and disgust are essential in maintaining tension and unease during narratives but are typically resolved by the end, reflecting catharsis or resolution for audiences.

2. *Surprise and Neutral*:
   - *Surprise* follows a unique trajectory, starting with very low normalized intensity, showing multiple peaks throughout the evolution of the timesteps, and ending with a middle intensity.  
     *Interpretation*: Surprise acts as a dynamic element, punctuating the narrative with moments of unexpected turns before stabilizing toward the end. This mirrors its role in maintaining audience engagement and unpredictability.

   - *Neutral* starts low at the beginning, then remains relatively stable throughout the story, only to spike heavily at the end and finish with a very high normalized intensity score.  
     *Interpretation*: Neutral states serve as transitions or resting points in narratives but often dominate endings, reflecting closure or resolution.

3. *Final Convergence*:
   - In the later timesteps, most emotions converge toward lower normalized values, except for *joy* and *neutral*, which dominate the emotional spectrum as climaxes are reached.  
     *Interpretation*: This convergence highlights how narratives resolve emotional conflicts, leaving audiences with feelings of hope (joy) or stability (neutral).

#### Overall Interpretation:
This normalized analysis highlights the interplay and relative importance of different emotions across a narrative timeline:
- *Anger* and *fear* are central to maintaining emotional tension over time, while their resolution by the end aligns with the catharsis typical of storytelling.
- *Sadness* plays a pivotal role in emotional climaxes or dramatic peaks, often tied to critical story moments.
- *Joy* and *neutral* emotions dominate at the start and end, framing stories with positivity and resolution, even after emotionally intense arcs.
- The dynamic nature of *surprise* punctuates stories, contributing to unpredictability and engagement.

This pattern reflects the structure of many narratives, where lighter emotions provide balance, and darker emotions drive conflict, with resolution or positivity prevailing by the end.



# Emotions and genres

### Average analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/heatmap_avg_emotion.html" width="100%" height="500" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

#### Neo’s Analysis: Emotional Averages Across Genres  
As Neo dives into the Matrix of Emotions, he uncovers patterns that reveal how different genres evoke distinct emotional intensities. Here are his key insights:

1. *Disgust Peaks in Horror*:  
   Neo immediately notices that the emotion of *disgust* is most prevalent in the Horror genre, where its intensity far surpasses that in other genres. “Horror thrives on discomfort,” Neo remarks, “and disgust is a key driver of that visceral reaction.”

2. *Sadness Dominates Drama and Romance*:  
   In both Drama and Romance, *sadness* emerges as a defining emotion, with the highest average intensities compared to other emotions. 

3. *Joy Shines in Comedy*:  
   The Comedy genre sees *joy* as its most prominent emotion, reflecting its purpose of uplifting and entertaining audiences of all ages.

4. *Fear in Horror and Thriller*:  
   Unsurprisingly, *fear* is most intense in the Horror and Thriller genres. While horror focuses on dread and terror, thrillers use fear to build tension and suspense. “These genres rely on keeping audiences on the ed  

### Visualizing Emotional Arcs by Genre

To visualize emotional trajectories, Neo plotted the normalized emotional arcs for each genre over 20 timesteps. 

<iframe src="{{ site.baseurl }}/assets/plots_alix\continentvsgenres.html" width="100%" height="600" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>


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

# Emotions and continents

### Average analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/heatmap_avg_continent.html" width="100%" height="500" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

Neo examines the heatmap of emotional intensity across continents, uncovering fascinating regional patterns:  

- *Anger* is most intense in African, North Americans and Asian films, while more moderate in South American, European and Oceanian productions.  
- *Disgust* stands out in African, European and South American films, with lower levels in Asian, North American and Oceanian cinema.
- *Fear* remains consistent globally, slightly higher in European films but less prominent in North America.  
- *Joy* is subdued overall, with a slight peak in Asian cinema and notably low intensity in North American films.  
- *Sadness* is uniformly moderate to high across continents, with stronger presence in African and Asian productions.  
- *Surprise* is the least intense emotion worldwide, showing minimal variation across regions.  

Overall, African films exhibit high emotional intensity, North American films lean toward restraint, Asian cinema emphasizes contrasts with negative and positive emotions quite high, and European productions balance their emotional palette. These variations reflect cultural nuances in global storytelling.

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/emotionsvscontinents.html" width="100%" height="500" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

Neo made it possible to also visualize this on a map for better understanding.

rajouter graphe en fonction des différents continents, voir si arcs varient selon continent 

Add oracle intro -->

## **Do longer movies tell more complex emotional stories?**

As Neo navigates through streams of data, this new question lingers in his mind. It resonates with him on a deeper level: 

Movies have the power to evoke a spectrum of emotions, from joy and sadness to anger and surprise. But does the length of a movie influence how complex its emotional journey can be? In this analysis, Neo explores whether longer movies, with runtimes exceeding 2 hours, exhibit more intricate emotional arcs compared to their shorter counterparts. By analyzing emotional metrics derived from sentiment analysis, Neo investigates the relationship between runtime and emotional storytelling.

Neo, as usual, dives into the data with his characteristic curiosity, seeing the emotional journey of each movie as a code waiting to be cracked.



## Results

### Emotional Complexity vs Runtime

When comparing emotional complexity metrics (amplitude, standard deviation, and sum of absolute changes) between short and long movies, Neo observed that:

- Long movies showed slightly higher variability in emotional arcs, but the differences were modest.
- Emotional complexity appeared to be influenced by factors beyond runtime, such as genre and storytelling style.

<iframe src="{{ site.baseurl }}/assets/plot/emotional_arcs_in_movies\mean_emotional_variation.png" width="100%" height="600" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

These results were not enough for Neo to conclude that longer movies inherently have more variation in emotional arcs or a more complex storyline. He decided to dive deeper by analyzing each emotion individually.

### Correlation Analysis

Neo computed the correlation between runtime and emotional complexity metrics for each emotion:

<iframe src="{{ site.baseurl }}/assets\plot\emotional_arcs_in_movies\emotional_complexity_emotions.png" width="100%" height="600" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

The correlation varied depending on the emotion considered. The highest correlation was for disgust, suggesting that as the movie length increases, the variation in this emotion also increases, leading to more emotional complexity. There were notable differences in correlation for emotions like anger, disgust, joy, and neutral, while fear, sadness, and surprise showed very low correlation between runtime and emotional variation.


The correlation was positive but weak (r ≈ 0.15), suggesting that while runtime contributes to emotional complexity, other narrative elements play significant roles.

Neo's analysis revealed that while longer movies tend to exhibit slightly more complex emotional arcs, runtime alone does not fully account for emotional storytelling.
Neo reflected on this, thinking about how a movie’s emotional depth cannot be reduced to just its runtime. There’s more to the emotional storytelling—something hidden in the layers of the plot, the pacing, and the way the characters evolve.

But there it is, Neo’s analysis is done. He's finished—for now. Or is he?

<iframe src="{{ site.baseurl }}/assets\images\Trinity.webp" width="50%" height="350" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>
Here comes Trinity. She’s not done yet. With a sharp look and a gun in hand, she’s demanding more. "Analysis. Do it by something other than genre. Now."

Looks like Neo has no choice. He’s about to dive back in—whether he likes it or not. 

Red pill, blue pill, en fonction de PCA et shape (ines) 

<div class="dropdown-container-blue">
  <button class="dropdown-btn-blue">Take the blue pill</button>
  <div class="dropdown-content-blue">
     
    {% capture markdown_content %}
## **Can we classify films by anything other than genre?**
As Neo dive back in the data, the question arises: Can emotions help us discover hidden trends in movies? Are North American drama films emotionally similar to European thrillers? Let's dive into his analysis and see what emerges.

Neo starts by looking at the Elbow Method and Silhouette Score graphs, from whom he can draw a few conclusions about clustering films by emotion:

- **Elbow Method**: The graph shows a sharp drop in inertia from 2 to 4 clusters, followed by a more gradual decrease. The "elbow" appears around 4-5 clusters, suggesting that this is the optimal number for the dataset.

- **Silhouette Score**: The scores, ranging from 0.13 to 0.17, indicate that the clusters overlap and aren't well-separated. The score peaks at 6-7 clusters, but declines sharply after that.

Combining both methods:
- The Elbow Method suggests 4-5 clusters for computational efficiency, while the Silhouette Score favors 6-7 for better-defined clusters.
- This suggests that emotions in films overlap naturally, reflecting how movies often evoke multiple emotions at once.

Neo finds that having 7 clusters fits perfectly for the analysis as each cluster represents a category of films that is emotionally dominated by one particular feeling. For example, cluster 1 is filled with films that evoke the most anger, cluster 2 showcases films that generate the most joy, and so on.

    {% endcapture %}
    {{ markdown_content | markdownify }}

  <iframe src="{{ site.baseurl }}/assets/plot/cluster/elbow_silhouette.html" width="100%" height=430px frameborder="0"></iframe>

    {% capture markdown_content %}
Neo also plots the clustering through K-Means of the seven emotions in 3D for better visualization. (Analyse????)
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/pca_kmeans.html" width="100%" height="900" frameborder="0"></iframe> 

    {% capture markdown_content %}
Neo takes a closer look at the data through clustering analysis. 
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/barplot_highest_emotions.html" width="100%" height="800" frameborder="0"></iframe>

    {% capture markdown_content %}
From here, Neo notices some interesting trends. Compared to the overall genre distribution, Action and Thriller films are overrepresented in clusters dominated by anger. In films where joy is most prevalent, there’s a notable overrepresentation of Drama, Romance, and Comedy films, while Thrillers and Horror films don’t show much joy. Comedy and Animation films tend to dominate when surprise is the most prominent emotion. Similar to cluster 2, films with high sadness are predominantly Drama and Romance. In cluster 5, which focuses on fear, Neo observes that Thrillers and Horror films are well-represented. Horror films also dominate when disgust is the most prevalent emotion. Finally, the cluster with the highest representation of Comedy, Family/Animation, and Fantasy-Sci-Fi films aligns with a more neutral emotional profile.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/repartition_overall_and_cluster.html" width="100%" height="700" frameborder="0"></iframe> 

    {% capture markdown_content %}
Neo also looked at how each genre is partitioned between different cluster to better understand the overall distribution of clusters across categories. These graphs supports Neo's analysis from above.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_per_category.html" width="100%" height="1600" frameborder="0"></iframe>

    {% capture markdown_content %}
## Analysis of Cluster Distribution by Genre and Emotions

### Cluster 1 - Anger
- **Highest proportion of anger**: *30.3% in Action/Adventure*, *26.5% in Thriller*.  
- **Neo's Analysis**:  
Action and adventure films generate anger primarily through themes of conflict, rivalry, and injustice. Physical confrontations, chases, and revenge-driven plots are hallmarks of the genre, evoking strong emotional reactions.  
In dramas, anger arises from frustration caused by unjust or tragic situations faced by the characters. This often reflects the audience's identification with societal, familial, or personal conflicts.
### Example: 
    {% endcapture %}
    {{ markdown_content | markdownify }}
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_1.html" width="100%" height="700" frameborder="0"></iframe>

    {% capture markdown_content %}
### Cluster 2 - Joy
- **Highest proportion of joy**: *13.7% in Comedy*, *20% in Romance*.  
- **Neo's Analysis**:  
While comedies aim to evoke joy, the proportion remains relatively low (13.7%), likely because humor is often intertwined with surprise or neutral elements, creating a mixed emotional experience.  
In romances, joy is more prominent (20%) as these films focus on moments of happiness, fulfilled love, and positive resolutions of relational conflicts.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_2.html" width="100%" height="700" frameborder="0"></iframe> 

    {% capture markdown_content %}
### Cluster 3 - Surprise
- **Highest proportion of surprise**: *11.3% in Family/Animation*, *9.89% in Comedy*.  
- **Neo's Analysis**:  
Family/animation and fantasy/science fiction films thrive on imaginative worlds, unexpected plot twists, and visually spectacular elements. These genres cultivate curiosity and wonder, which are core components of surprise.  
Plot reversals and magical or futuristic scenarios encourage viewers to explore new possibilities, evoking both surprise and fascination.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_3.html" width="100%" height="700" frameborder="0"></iframe>
    
    {% capture markdown_content %}
### Cluster 4 - Sadness
- **Highest proportion of sadness**: *20.7% in Romance*, *19.5% in Drama*.  
- **Neo's Analysis**:  
Dramas delve into emotions of loss, hardship, and human sacrifice, often presenting realistic emotional conflicts that evoke authentic sadness in viewers.  
Romances, while generating joy, also explore themes of heartbreak, unfulfilled love, or emotional dilemmas, leading to sadness when relational conflicts remain unresolved.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_4.html" width="100%" height="700" frameborder="0"></iframe>

    {% capture markdown_content %}
### Cluster 5 - Fear
- **Highest proportion of fear**: *29.7% in Horror*, *20.2% in Thriller*, *19.2% in Fantasy/Sci-Fi*.  
- **Neo's Analysis**:  
Horror films evoke primal fear and anxiety through themes of survival, imminent danger, or supernatural elements. Psychological theories suggest fear triggers strong physiological responses (adrenaline and muscle tension), enhancing audience immersion.  
Thrillers induce a more cognitive form of fear, relying on suspense, hidden threats, and plot twists to maintain a state of tension and unease.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_5.html" width="100%" height="700" frameborder="0"></iframe>

    {% capture markdown_content %}
### Cluster 6 - Disgust
- **Highest proportion of disgust**: *30.3% in Horror*.  
- **Neo's Analysis**:  
Horror films often elicit disgust through graphic, violent, or disturbing imagery. Disgust is tied to instinctual reactions of repulsion and self-preservation, amplifying the sensory impact of the viewing experience.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_6.html" width="100%" height="700" frameborder="0"></iframe>

    {% capture markdown_content %}
### Cluster 7 - Neutral
- **Highest proportion of neutrality**: *40.5% in Family/Animation*, *35.5% in Fantasy/Sci-Fi*.  
- **Neo's Analysis**:  
Family and comedy films tend to avoid extreme emotions, opting for light, balanced narratives that are accessible to broader audiences. This emotional neutrality reflects a desire to provide positive experiences without overwhelming viewers.
    {% endcapture %}
    {{ markdown_content | markdownify }}

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_7.html" width="100%" height="700" frameborder="0"></iframe>
  </div>
</div>

<div class="dropdown-container-red">
  <button class="dropdown-btn-red">Take the red pill</button>
  <div class="dropdown-content-red">
      
  </div>
</div>

## General Conclusion

Neo's analysis of film clusters and their dominant emotions highlights a strong correlation between genres and emotional experiences, aligning with emotion theory:

- **Negative Emotions** (anger, sadness, fear, disgust):  
  - Predominant in *drama*, *thriller*, and *horror* genres, which explore themes of tension, loss, and threat.  
  - These emotions often provide catharsis for the audience and deepen immersion into the narrative.  

- **Positive Emotions** (joy, surprise):  
  - Prevalent in *comedy*, *romance*, and *family/animation* genres, which aim to create lighthearted, enjoyable, or awe-inspiring experiences.  
  - Optimistic storytelling and visually enchanting worlds help stimulate positive emotional responses.

- **Emotional Neutrality**:  
  - Associated with *family* and *comedy* films, neutrality allows for accessible, emotionally balanced content suited for a wide audience.  

### Summary  
Neo concludes that the clusters reflect an emotional specialization within film genres. Each genre serves a unique emotional purpose, eliciting specific psychological and physiological responses in viewers. This diversity underscores cinema's powerful ability to provoke varied and complex emotional reactions.  

## General Conclusion

### 1. Data Collection and Categorization

Neo used movie summaries from the CMU Movie Summary Corpus and was provided with additional data scraped from Wikipedia. Each movie was tagged with its primary genre(s), enabling Neo to group emotional arcs by genre for comparative analysis. 

Because of the astronomic number of genres in the data (about 360), Neo decided to handcraft a mapping to go down from 300 plus genres of movies to about a dozen. While Neo's mapping may be a point of discussion among movie enthousiasts, Neo find it a good approximation to a more general genre classification. 

Neo pauses. “Reduction,” he murmurs. “Finding simplicity in the noise. It’s like filtering out the static in the Matrix.”


Neo first take a look at the genres distribution in films.
Drama is the most common genre, accounting for the largest proportion at approximately 26%. This is followed by comedy and thriller, which hold significant but smaller shares. The distribution suggests a diverse set of genres without a single dominant category, reflecting the varied preferences in cinematic storytelling. 

Neo smirks. “Drama. Of course. Conflict defines us, doesn’t it? The choices we make, the consequences we endure. But diversity in stories… that’s the humanity behind it all.”

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
<style>
/* Dropdown container */
/* Dropdown container */
.dropdown-container-blue {
  position: relative;
  margin: 20px 0;
}

/* Dropdown button */
.dropdown-btn-blue {
  background-color: rgb(0, 8, 255);
  color: white;
  padding: 10px 20px;
  border: 4px solid rgb(0, 8, 255);
  cursor: pointer;
  font-size: 16px;
  font-weight: 600;
  height: 48px;
  justify-content: center;
  letter-spacing: -.8px;
  line-height: 24px;
  border-radius: 5px;
  width: 100%;
  height: 48px;
  box-sizing: border-box;
  font-family: Inter, sans-serif;
  text-align: center;
  transition: background-color 0.3s ease;
}

.dropdown-btn-blue:hover {
  background-color: rgb(4, 1, 158);
}

/* Dropdown content */
.dropdown-content-blue {
  display: flex;
  flex-direction: column;
  align-items: center; /* Center content horizontally */
  text-align: left;
  padding: 20px;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 5px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Center iframe specifically */
.dropdown-content-blue iframe {
  display: block;
  margin: 20px auto; /* Center the iframe and add spacing */
  max-width: 100%;
  align-items: center;
  align-text: center;
}

/* Dropdown button */
.dropdown-btn-red {
  background-color:rgb(255, 47, 0);
  color: white;
  padding: 10px 20px;
  border: 4px solid rgb(255, 47, 0);
  cursor: pointer;
  font-size: 16px;
  font-weight: 600;
  height: 48px;
  justify-content: center;
  letter-spacing: -.8px;
  line-height: 24px;
  border-radius: 5px;
  width: 100%;
  height: 48px;
  box-sizing: border-box;
  font-family: Inter, sans-serif;
  text-align: center;
  transition: background-color 0.3s ease;
}

.dropdown-btn-red:hover {
  background-color:rgb(173, 36, 5);
}


/* Dropdown content */
.dropdown-content-blue {
  display: none;
  margin-top: 10px;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 5px;
  padding: 15px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

/* Show dropdown when open */
.dropdown-container-blue.open .dropdown-content-blue {
  display: block;
}

/* Dropdown content */
.dropdown-content-red {
  display: none;
  margin-top: 10px;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 5px;
  padding: 15px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

/* Show dropdown when open */
.dropdown-container-red.open .dropdown-content-red {
  display: block;
}


</style>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    document.querySelectorAll(".dropdown-btn-red").forEach(function (btn) {
      btn.addEventListener("click", function () {
        const container = this.parentElement;
        container.classList.toggle("open");
      });
    });
  });
</script>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    document.querySelectorAll(".dropdown-btn-blue").forEach(function (btn) {
      btn.addEventListener("click", function () {
        const container = this.parentElement;
        container.classList.toggle("open");
      });
    });
  });
</script>
