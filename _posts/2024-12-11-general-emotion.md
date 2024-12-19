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

<div class="dropdown-buttons">
  <div class="dropdown-container-blue">
    <a href="/dataffoneurs-story/mediator/feature/2024/12/11/bluepill.html" id="bottom" class="dropdown-btn-blue">Take the blue pill</a>
  </div>
  <br>
  <div class="dropdown-container-red">
    <a href="/dataffoneurs-story/mediator/feature/2024/12/11/redpill.html" class="dropdown-btn-red">Take the red pill</a>
  </div>
</div>
<br>

<style>
/* Blue button style */
.dropdown-btn-blue {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background-color: rgb(0, 68, 255);
  border: 2px solid #000;
  box-sizing: border-box;
  color: #fff; !important/* Text in white */
  cursor: pointer;
  font-family: Inter, sans-serif;
  font-size: 16px;
  font-weight: 600;
  height: 48px;
  width: 100%; /* Take full width */
  padding: 0 17px;
  text-align: center;
  text-decoration: none; /* Remove underline */
  transition: all 0.3s ease;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.dropdown-btn-blue:hover {
  background-color: rgb(4, 1, 158); /* Change background to darker blue on hover */
  color: #fff; /* Ensure text stays white on hover */
}

/* Red button style */
.dropdown-btn-red {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background-color: rgb(234, 11, 11);
  border: 2px solid #000;
  box-sizing: border-box;
  color: #fff; !important /* Text in white */
  cursor: pointer;
  font-family: Inter, sans-serif;
  font-size: 16px;
  font-weight: 600;
  height: 48px;
  width: 100%; /* Take full width */
  padding: 0 17px;
  text-align: center;
  text-decoration: none; /* Remove underline */
  transition: all 0.3s ease;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.dropdown-container-blue a.dropdown-btn-blue {
  text-decoration: none; /* Ensure underline is removed */
  color: #fff !important; /* Force white text */
}

.dropdown-btn-red:hover {
  background-color: rgb(173, 36, 5); /* Change background to darker red on hover */
  color: #fff; /* Ensure text stays white on hover */
}

.dropdown-container-red a.dropdown-btn-red {
  text-decoration: none; /* Ensure underline is removed */
  color: #fff !important; /* Force white text */
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
