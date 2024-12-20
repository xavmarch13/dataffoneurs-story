---
layout: post
title:  "Neo's journey through emotion: uncovering patterns in film sentiment"
weight:  3
categories: [Data Analysis, Sentiment Analysis, Movies]
tags: featured
image: /assets/images/xUtR9aTaqj4XTDDUgWwTrC.jpg
image2: /assets/images/xUtR9aTaqj4XTDDUgWwTrC.jpg
previous_post: /dataffoneurs-story/data analysis/sentiment analysis/movies/2024/12/11/how-to-get-emotions.html
next_post: /dataffoneurs-story/jekyll/update/2024/12/11/welcome-to-jekyll.html
---

# The emotional journey

Emotions are the backbone of cinematic storytelling, captivating audiences and leaving lasting impressions. But do these emotional arcs follow universal patterns, or are they tailored to fit specific genres? In this post, we dive into emotional trajectories across different movie genres, using sentiment analysis to uncover whether genre dictates the emotional journey of a film.

Neo, the legendary hacker from The Matrix, finds himself reflecting on this question while navigating through streams of data. The question resonates with him deeply. After all, isn’t every journey—a story? Whether it’s dodging bullets or defying fate, Neo knows better than most that patterns are everywhere, even in the emotions that drive our stories forward.

Neo peers at the data flowing past him, an ocean of emotional peaks and valleys. To uncover meaning, he realizes, the system must be broken down into its parts—categorizing genres, tracing patterns, and finding anomalies.

Neo delves into the Matrix of Emotions to uncover the answers, guiding us through the data analysis that reveals how emotions shift across cinematic genres.

# Global emotional trends

### Average analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/average_emotion_intensity_across_movies.html" width="100%" height="625" frameborder="0" style="max-width: 100%; border-left: 150px solid white;"></iframe>

Peering into the digital fabric of the boxplot data, Neo questions the anomaly: why does an emotion as peculiar as disgust surge with such intensity? The Matrix reveals a clue—neutral and disgust are linked by a negative correlation of -0.428 (p-value = 0). This connection, etched into the data, hints at an unseen balance between emotional extremes. With this initial revelation, Neo begins to decode the deeper patterns hidden within the emotional construct.
### Neo’s observations: the emotional code deciphered

1. **Neutral as the anchor of the system**: Neo notes that neutrality dominates as the most frequent emotion, with a wide range and numerous outliers. “Neutrality,” Neo reflects, “is the backbone of every story—a stable framework that lets other emotions rise and fall.”
2. **Disgust commands the stage**: Disgust emerges as a forceful emotion, with its consistent intensity marking it as a driver of conflict. “Disgust exposes flaws,” Neo muses, “forcing characters and audiences to confront what’s wrong.”
3. **Sadness and anger: the emotional tug of war**: Neo observes their intertwined distributions. Sadness fosters introspection, while anger drives external action. “Together,” Neo concludes, “they break and build—key forces in shaping narratives.”
4. **Fear looms over joy**: Fear is more persistent, subtly driving tension throughout the story. Joy, while impactful, offers brief relief. “Fear sets the stakes,” Neo notes, “and joy is the reward.”
5. **Surprise: the system’s glitch**: Surprise, though minimal in intensity, disrupts predictability with sudden spikes. “It’s the system’s glitch,” Neo says. “Small but essential to keeping narratives dynamic.”

### Time-series analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/normalised_emotions_time_analysis.html
" width="95%" height="625" frameborder="0" style="max-width: 100%; border-left: 150px solid white;"></iframe>


#### Neo’s observations: decoding the emotional matrix 
   Neo stares into the data, the emotional arcs forming lines of code in his mind.  
   - **Anger** grows steadily with tension, peaking mid-story and fading in resolution.
   - **Joy** bookends narratives, peaking at the start and end. 
   - **Sadness** rises early, peaks during the climax, and dissipates in resolution.
   - **Fear** and **disgust** dominate early, creating tension, but fade as resolution near.
   - **Surprise** disrupts the story unpredictably, spiking throughout the narrative.
   - **Neutral** grows steadily, peaking in resolution.

  “This is how stories end,” Neo observes. “Conflict fades, tension resolves, and what’s left is either hope or balance. The system restores itself, leaving us with peace or satisfaction.”

Neo smirks as he looks at the data. “This isn’t just a pattern,” he says. “It’s the blueprint of the human condition, a reflection of how we navigate chaos, find meaning in conflict, and restore balance to our own systems.”  

# Emotions and genres

### Average analysis

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/heatmap_avg_emotion.html" width="100%" height="625" frameborder="0" style=" border-left: 170px solid white;"></iframe>

#### Neo’s analysis: emotional averages across genres  
As Neo dives into the Matrix of Emotions, he uncovers patterns that reveal how different genres evoke distinct emotional intensities. Here are his key insights:

1. **Disgust Peaks in Horror**:  
   Neo immediately notices that the emotion of **disgust** is most prevalent in the Horror genre, where its intensity far surpasses that in other genres. “Horror thrives on discomfort,” Neo remarks, “and disgust is a key driver of that visceral reaction.”

2. **Sadness Dominates Drama and Romance**:  
   In both Drama and Romance, **sadness** emerges as a defining emotion, with the highest average intensities compared to other emotions. 

3. **Joy Shines in Comedy**:  
   The Comedy genre sees **joy** as its most prominent emotion, reflecting its purpose of uplifting and entertaining audiences of all ages.

4. **Fear in Horror and Thriller**:  
   Unsurprisingly, **fear** is most intense in the Horror and Thriller genres. While horror focuses on dread and terror, thrillers use fear to build tension and suspense. “These genres rely on keeping audiences on the ed  

### Visualizing emotional arcs by genre

To visualize emotional trajectories, Neo plotted the normalized emotional arcs for each genre over 20 timesteps across all continents. 

<iframe src="{{ site.baseurl }}/assets/plots_alix\emotionvsgenres.html" width="110%" height="830" frameborder="0" style="max-width: 110%; display: block; margin-left:auto; margin-right: auto"></iframe>

### The consistent rhythm of emotional arcs across genres    

### Universal vs. Genre-specific emotional patterns  
Neo identifies three emotions—anger, joy, and disgust—that seem to transcend genre boundaries.

Neo's analysis reveals that some emotions, such as anger, joy, and disgust, follow very similar trajectories regardless of the genre. In contrast, emotions like fear, sadness, and surprise show significant variability depending on the type of story being told.

Joy usually starts high, then drops as we move further in the story, only to rise back up at the end, reflecting resolution

But Neo, ever the questioner, probes further. Why do some genres, like Horror or Romance, deviate from this structure? The answer lies in how emotions function within different storytelling frameworks and this distinction can be understood by examining the **storytelling conventions** and the **inherent characteristics** of these emotions. 

This universal structure suggests that filmmakers rely on common narrative techniques to captivate audiences across different genres.  

### **1. The universal role of joy, anger, and disgust**  

- **Joy and anger as narrative pillars:**  

  Neo realizes that filmmakers use emotions strategically to meet audience expectations:

  Joy and anger are universal emotions that frequently shape the core of cinematic storytelling. **Joy** usually starts high, then drops as we move further in the story, only to rise back up at the end, reflecting resolution, triumph, or humor, while **anger** starts low only to rise during the movie, to finally drops back down at the end, reflecting that anger grows during moments of conflict, betrayal, or injustice in the middle of the movie, and drop at the end when there's triumph, resolution or humor. These elements are staples of nearly every genre, ensuring that joy and anger arcs remain largely consistent across diverse narratives. These emotions mirror Neo’s journey through struggle, revelation, and triumph.

- **Disgust’s steady arc across genres:**  
  Unlike more dynamic emotions, **disgust** tends to play a subtler, secondary role in storytelling. Disgust generally follows an emotional arcs that grows in the middle of the movie, showing disgust as conflict and challenges arises in the middle of the movie. It often manifests in reaction to specific events—such as repugnant behavior or unsettling scenarios—rather than driving the story forward. It then falls off in the second half of the movie to finally have practically no disguts. This situational nature results in a stable arc for disgust across genres, with minimal variations  

- **Narrative archetypes and consistency:**  
  Across genres, many stories follow shared archetypes, such as the "hero's journey," which naturally incorporates anger, disgust, and joy. These emotions mark key stages in the narrative: anger during challenges, disgust when confronting unpleasant truths, and joy at the resolution of the conflict. Their consistent presence underscores their foundational role in storytelling.  

### **3. Emotional functions in storytelling**  

- **Primary vs. contextual emotions:**  
  Neo finds that motions like anger, joy, and disgust serve as "primary emotions", essential for driving the plot and defining key narrative moments. On the other hand, fear, sadness, and surprise act as "contextual emotions," their intensity and role dictated by the genre’s tone and purpose.  

- **Meeting audience expectations:**  
  Audience expectations also play a significant role in shaping emotional arcs. For example, horror audiences anticipate fear and surprise, while drama viewers expect a mix of sadness and joy. Disgust, meanwhile, serves as a versatile tool across genres, punctuating specific scenes without dominating the narrative.  

### **Conclusion**  

Much like Neo’s journey, the emotional arcs of movies reflect both universal truths and unique challenges. The universality of emotions like anger, joy, and disgust reflects their foundational role in storytelling, while the variability of emotions like fear, sadness, and surprise highlights the creative flexibility filmmakers employ to craft genre-specific narratives.

# Emotions and continents

### Average analysis
<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/heatmap_avg_continent.html" width="100%" height="620" frameborder="0" style="max-width: 100%; border-left: 170px solid white;"></iframe>

Neo examines the heatmap of emotional intensity across continents, uncovering fascinating regional patterns:  

- **Anger** is most intense in African, North Americans and Asian films, while more moderate in South American, European and Oceanian productions.  
- **Disgust** stands out in African, European and South American films, with lower levels in Asian, North American and Oceanian cinema.
- **Fear** remains consistent globally, slightly higher in European films but less prominent in North America.  
- **Joy** is subdued overall, with a slight peak in Asian cinema and notably low intensity in North American films.  
- **Sadness** is uniformly moderate to high across continents, with stronger presence in African and Asian productions.  
- **Surprise** is the least intense emotion worldwide, showing minimal variation across regions.  

Overall, African films exhibit high emotional intensity, North American films lean toward restraint, Asian cinema emphasizes contrasts with negative and positive emotions quite high, and European productions balance their emotional palette. These variations reflect cultural nuances in global storytelling.

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/emotionsvscontinents.html" width="100%" height="620" frameborder="0" style="max-width: 100%; border-left: 50px solid white;"></iframe>

Neo made it possible to also visualize this on a map for better understanding.

<iframe src="{{ site.baseurl }}/assets/plots_alix\continentvsgenres.html" width="110%" height="830" frameborder="0" style="max-width: 110%; display: block; margin-left:auto; margin-right: auto"></iframe>

Neo dives into the emotional arcs across genres, this time examining variations by continent. The findings reveal fascinating contrasts:

Some continents, such as **North America**, **Asia**, and **Europe** exhibit a more consistent emotional arc across genres for certain emotions such as joy, anger and disgust. These arcs closely resemble the average emotional trajectory observed when considering all continents combined, suggesting a stronger alignment with global storytelling trends. 

In contrast, continents like **Africa**, **Oceania** and **South America**, display highly diverse emotional arcs that vary significantly between genres, even for emotions such as joy, anger and disgust. There is no single dominant pattern for each emotions; instead, the arcs shift dramatically depending on the storytelling style and thematic focus of each genre.   

These results could be related to the lower number of movies in Oceania, South America, and Africa, which could explain the observed variations, but this also highlights how cultural influences shape emotional storytelling, with some regions embracing genre-specific emotional diversity and others leaning toward a unified narrative rhythm across genres.

--- 

**The Oracle appears, her calm yet cryptic demeanor radiating wisdom. She smiles knowingly and leans forward, speaking in her usual enigmatic tone:**  

<iframe src="{{ site.baseurl }}/assets/images\Neo-and-The-Oracle-in-The-Matrix-Reloaded.png" width="100%" height="800" frameborder="0" style="max-width: 100%; border-left: 100px solid white;"></iframe>

"Ah, you've come far in understanding emotions and stories. But let me ask you something new, something unexpected…" 
## **Do longer movies tell more complex emotional stories?**

Her words hang like a riddle, challenging Neo to think deeper. She tilts her head, her smile widening, as if she already knows the answer—but leaves it for Neo to uncover. As Neo delves into streams of data, the Oracle's question lingers in his mind, pushing him to uncover its answer.

Movies have the power to evoke a spectrum of emotions, from joy and sadness to anger and surprise. But does the length of a movie influence how complex its emotional journey can be? In this analysis, Neo explores whether longer movies, with runtimes exceeding 2 hours, exhibit more intricate emotional arcs compared to their shorter counterparts. By analyzing emotional metrics derived from sentiment analysis, Neo investigates the relationship between runtime and emotional storytelling.

Neo, as usual, dives into the data with his characteristic curiosity, seeing the emotional journey of each movie as a code waiting to be cracked.

### Calculating emotional etrics
To quantify emotional complexity, Neo computed two key metrics for each movie:

- **Standard deviation:** The variability of emotion intensity throughout the plot.
- **Sum of absolute changes:** The cumulative magnitude of emotion shifts between consecutive timesteps.

## Results
### Emotional complexity vs runtime

When comparing emotional complexity metrics (standard deviation and sum of absolute changes) between short and long movies, Neo observed that:

- Long movies showed slightly higher variability in emotional arcs, but the differences were modest.
- Emotional complexity appeared to be influenced by factors beyond runtime, such as genre and storytelling style.

<iframe src="{{ site.baseurl }}/assets/plot/emotional_arcs_in_movies\emotional_variation_by_film_length.html" width="100%" height="600" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

These results were not enough for Neo to conclude that longer movies inherently have more variation in emotional arcs or a more complex storyline. He decided to dive deeper by analyzing each emotion individually.

### Correlation analysis
Neo computed the correlation between runtime and emotional complexity metrics for each emotion:

<iframe src="{{ site.baseurl }}/assets\plot\emotional_arcs_in_movies\correlation_emotional_variation.html" width="100%" height="600" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

The correlation varied depending on the emotion considered. The highest correlation was for disgust, suggesting that as the movie length increases, the variation in this emotion also increases, leading to more emotional complexity. There were notable differences in correlation for emotions like anger, disgust, joy, and neutral, while fear, sadness, and surprise showed very low correlation between runtime and emotional variation.

The correlation was positive but weak (r ≈ 0.15), suggesting that while runtime contributes to emotional complexity, other narrative elements play significant roles.

Neo's analysis revealed that while longer movies tend to exhibit slightly more complex emotional arcs, runtime alone does not fully account for emotional storytelling.
Neo reflected on this, thinking about how a movie’s emotional depth cannot be reduced to just its runtime. There’s more to the emotional storytelling—something hidden in the layers of the plot, the pacing, and the way the characters evolve.

---
Neo sits quietly, the faint hum of data streams echoing in the background, when Morpheus steps into the scene, his silhouette commanding attention. His voice is calm but laced with purpose.

<iframe src="{{ site.baseurl }}/assets\images\large_landscape_175005.webp" width="100%" height="750" frameborder="0" style="max-width: 100%; display: block; margin-left:auto; margin-right: auto"></iframe>

“Neo,” he says, holding out his hands, “this is the moment of choice. In my right hand, the **red pill**—a journey into the world of **K-Shape clustering**. You’ll embrace the dynamic nature of time-series patterns, finding clusters that capture the rhythm and evolution of emotional arcs."
He pauses, shifting his gaze to the left. “In my left hand, the **blue pill**—**PCA clustering**. A method of elegant simplicity, reducing dimensions to their essence. Here, patterns emerge in a structured space, but you’ll miss the nuance of how emotions evolve moment by moment.”

Morpheus steps closer, his eyes piercing. “Choose wisely. The **red pill** dives into complexity, embracing the chaos of storytelling arcs. The **blue pill** offers clarity, a streamlined view of emotional trends. Either way, the data will reveal its secrets—but only one path leads to the full depth of the narrative.”

Neo hesitates, his gaze flicking between the two pills. What will he choose? The structured elegance of PCA clustering or the intricate adaptability of K-Shape clustering? The journey into emotional analysis awaits. 


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
