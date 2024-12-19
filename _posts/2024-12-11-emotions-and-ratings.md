---
layout: post
title:  "7. BARBIE does analysis between emotions and ratings"
weight: 7
date:   2024-12-11 11:08:25
categories: emotions and ratings
tags: featured
---

DO barbie style, barbie does the movie rating analysis

associate to each category an emotion
see the mean rating of movies according to their categories
if horror very low rated --- less horror films produced, smaller sample --- horror dominated by emotion fear
fear is less prevalent in continents where percentage of horror less small
> [CLOSING VISUALIZATION: A "Genre Emotional Complexity Score" infographic ranking genres by their emotional range and variation]


## Introduction

The essence of cinema lies in its ability to evoke and explore the depths of human emotion, serving as a mirror to our shared experiences and inner lives. Emotions in movies transcend mere storytelling, becoming a universal language that connects us to characters, moments, and each other. They reveal the complexities of existence, illuminating joy, sorrow, love, and conflict in ways that words alone cannot. 

In this section, we embark on a journey to decipher/unravel the intricate relationship between emotions and a movie's success, focusing specifically on how they influence viewer ratings. Delving deeper, we seek to uncover not only the presence of emotions but also their dynamics — exploring how these emotional elements contribute to shaping audience reception and appraisal.
Through this lens, we aim to illuminate the emotional alchemy that lies at the heart of cinematic triumph.


In the following we will attempt to provide an intuition to the myriad of questions such as:
- What emotions do we seek to experience on the big screen? What are the essential emotional ingredients required to satisfy our soul’s cinematic hunger?
- Does a more varied emotional journey lead to higher ratings? Do movies with multiple emotions expressed throughout the story garner higher success?
- MORE !!!!

## The Influence of Emotions in a Movie's Success

<br />

### How do ratings distribute across different movie categories?

First of all, we observe how the ratings differ across different movie categories. 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_by_category.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Dramas have the highest mean rating, which may reflect how this genre often deals with complex human experiences and social issues, as these films often explore universal themes (family, love, loss, identity) that resonate across cultural boundaries. (connection with dramas having more sadness -- dominant emotion with highest rating!)

Horror films have the lowest mean rating, which can be attributed to the genre's polarizing nature - people tend to either love or hate horror. Additionnaly, there may exist a cultural stigma around horror as a "less serious" genre. 

After seeing this first distinction with regards to categories, we can embark !!!


### Does a Movie's Primary Emotion Predict How Much We'll Like It?

We observe how the mean ratings differ between movies classified by their dominant emotion.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_per_dominant_emotion.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The analysis reveals statistically significant differences in movie ratings across different dominant emotions.

Movies dominated by **sadness** tend to receive the highest average ratings, followed by joy and anger. Films where **fear** is the dominant emotion received the lowest average ratings. Thus, a movie's dominant emotion does have a meaningful relationship with how audiences rate it.

To explain why sadness takes the lead, we might theorize that serious, emotionally heavy films frequently tackle complex social issues and human conditions, and so are often viewed as more "meaningful".

When breaking down this analysis by continent, only Asia and North America demonstrate statistically significant differences (as indicated by their ANOVA p-values) in how movies of different dominant emotions are rated. Between these two continents, there is an specially meaningful contrast in their reception of **disgust-dominant films**: while Asian audiences give these films their highest average ratings, North American viewers consistently rate them among their lowest. This remarkable disparity suggests fundamental differences in how these cultures process and value this specific emotional content in cinema.

Although these findings suggest that a movie's dominant emotion does influence movie ratings, the differences are relatively modest, hinting that the emotional landscape of cinema resists such simple categorization. Therefore, we adopt a more detailed approach and delve deeper into emotional diversity, that is, to what extent multiple emotions are expressed throughout a story.


### Does a More Varied Emotional Journey Lead to Greater Success?

One hypothesis is that movies with more dynamic and varied emotional arcs have a greater ability to resonate with a wider audience, in contrast to those with a more emotionally flat or one-dimensional narrative. This idea isn't new - as Stanley Kubrick observed:

> "A film is--or should be--more like music than like fiction. It should be a progression of moods and feelings."
>
> **Stanley Kubrick, acclaimed director**  

To quantify this "progression of moods and feelings" that Kubrick describes, we employed four distinct metrics:

1. **Shannon Entropy**: Measures the overall balance of emotions throughout the movie - higher values indicate a more even distribution across different emotions rather than dominance of just one or two
2. **Emotion Transitions**: Counts how often the dominant emotion changes, capturing the dynamic shifts in emotional tone
3. **Emotion Variation**: Measures the standard deviation of emotional intensities over time, showing how much emotions fluctuate
4. **Unique Dominant Emotions**: Simply counts how many different emotions take the lead at some point in the movie

We perform a general analysis of the ratings with the diversity metrics, and find the following correlations: 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_general_diversity.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Movies with more diverse and dynamic emotional content tend to receive slightly higher ratings, supporting the hypothesis that emotional variety resonates with audiences. However, the relatively small correlation coefficients suggest that while emotional diversity does play a role in audience reception, it's likely just one of many factors that influence overall movie ratings.

By continental regions, we can witness stronger correlations that may indicate geographical variations.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_continent_diversity.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

In **Europe and North America**, all metrics show consistent, statistically significant positive correlations with ratings. This suggests that Western audiences tend to rate movies more favorably when they feature more diverse emotional content.

**South America** shows the strongest positive correlations among all continents. This indicates that South American audiences may be particularly appreciative of emotionally diverse films, with **emotion transitions** having the strongest impact on ratings. This likely reflects deep cultural roots in melodramatic storytelling, particularly through telenovelas. **Telenovelas**, which originated in Latin America, are characterized by intense emotional oscillations and dramatic transitions. 

Asia presents an interesting case where emotion transitions show the strongest correlation with ratings, while other metrics have weaker relationships. This results reflect different cultural and cinematographic traditions, as in many East Asian countries, movies maintain consistent emotional tones within genres, e.g., consistent melancholy in many dramas, which may explain the unsignificant correlation with Shannon entropy.

Oceania and Africa were excluded from this analysis as their limited sample size may affect the statistical power of it. 

### Do we really want happy endings? The numbers tell a different story

> "Man only likes to count his troubles; he doesn’t calculate his happiness."
>
> **Fyodor Dostoevsky**

This observation from Dostoevsky about human nature's peculiar relationship with suffering might explain what we found when analyzing movie endings. To dig deeper into this question, we classify movies according to their ending, looking at the emotions in the last timestep. 

We first observe how these 'happy' ending and 'sad' endings movies are distributed across different categories: 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/distribution_by_category_and_ending.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Drama shows a significant skew towards sad endings, due to the fact that dramatic narratives often explore challenging themes and complex resolutions that don't always end cheerfully. Interestingly, Romance films maintain a fairly consistent presence across both categories, suggesting that while society often associates romance with "happily ever after," there's also a strong tradition of tragic love stories that resonates with audiences' understanding that relationships can be sources of both joy and heartbreak.

Looking at average ratings by category, depending on 'happy' or 'sad' endings, we find:

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/average_ratings_by_category_and_ending.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The relationship between ending type and audience reception is more complex than might be expected, and successful movies don't necessarily need to have happy endings to be well-received by audiences. The impact of ending type appears to be genre-dependent.

In Drama and Romance, movies with sad endings tend to receive slightly higher ratings than those with happy endings. This might suggest that audiences appreciate emotional depth and tragic elements in these genres, perhaps viewing them as more meaningful or artistically valuable
On the other hand, Fantasy/Sci-Fi shows a reverse pattern, where happy endings rate slightly higher than sad endings. 


### Emotion ARCS and ratings

> [INTERACTIVE ELEMENT SUGGESTION: Create a "Choose Your Own Emotional Adventure" graph where readers can click different emotional combinations to see what movie genres typically match those patterns]

With K-Shape clustering done for each emotion separately, we find the best and worst performing cluster for each movie category per emotion. 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/best_and_worst_clusters_general.html" 
    width="100%" 
    height="1400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The analysis of emotional arcs across different film genres reveals distinct patterns that contribute to their effectiveness. Each genre demonstrates unique requirements for emotional pacing and intensity, with some showing more sensitivity to specific emotions than others.

Action/Adventure films exhibit the most balanced emotional profile, requiring careful management of anger, fear, and sadness. These films succeed best when they maintain moderate baseline emotional intensity with strategic peaks, rather than constant high-intensity stimulation. This suggests that even action-packed narratives benefit from emotional breathing room that allows audiences to process and invest in the story.

> EXAMPLE OF FILM WITH (CLUSTER ANGER 1) (CLUSTER FEAR 1) (CLUSTER SADNESS 4)

Fantasy/Sci-Fi emerges as the most emotionally demanding genre, showing high deltas across all emotions. It is therefore the most polarizing genre emotionally. The most successful emotional arcs in this genre demonstrate gradual build-ups that allow audiences to acclimate to new worlds before reaching emotional peaks. This is particularly evident in fear arcs (Cluster 7), where a measured increase to a sustained mid-point peak proves more effective than rapid emotional spikes.

> EXAMPLE OF FILM WITH (FEAR ARC CLUSTER 7)  701775
<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_scifi_movie_fear_cluster7.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

> HORROR FEAR CLUSTER 2 27420904

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_horror_movie_fear_cluster2.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>


> ACTION/ADVENTURE SADNESS CLUSTER 4 28157443



<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_action_movie_sadness_cluster4.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>


Horror films show fascinating patterns in anger and surprise management. The most effective anger arc (Cluster 5) maintains a steady moderate intensity rather than dramatic spikes, suggesting that sustained tension outperforms shock value. Similarly, successful surprise arcs maintain consistent mid-level arousal with small variations, allowing for effective shock moments while avoiding emotional exhaustion.
Horror shows the largest deltas across multiple emotions (Anger, Fear, Surprise), suggesting it's one of the most emotionally polarizing genres. Psychological Theory: This aligns with the "Excitation Transfer Theory" where heightened arousal from fear/anxiety can intensify subsequent emotional responses. Cluster 5 being best for both Anger and Horror suggests successful horror relies on building tension through anger before releasing it through fear.

> : Create a side-by-side comparison of emotional arcs, like an EKG reading, showing the difference between a "jump scare" horror movie versus a "sustained tension" one (CLUSTER 5 ANGER) versus (CLUSTER 4 ANGER)
> CASE STUDY SUGGESTION: Add a breakdown of a critically acclaimed horror film that follows this pattern perfectly, showing the emotional data overlaid with key scene descriptions

For emotional arc characteristics across specific emotions:

Anger works best when it follows a gradual build-up pattern with sustained intensity (Cluster 5), particularly in horror films, as they need a consistent underlying tension. Failed anger arcs (Cluster 4) typically show early spikes followed by decline. This premature anger release undermines horror buildup.

Fear demonstrates optimal results with a gradual build to a mid-point peak followed by sustained elevation (Cluster 7). It is successful because it allows time for world-building before emotional peaks. Failed fear arcs show sharp initial spikes with steady declines (Cluster 6), suggesting that rapid emotional exhaustion prevents audience engagement. This is particularly crucial in fantasy/sci-fi, where world-building requires sustained emotional investment.


Sadness shows interesting patterns in Action/Adventure, where success comes from gradual decrease with multiple small peaks (Cluster 4) rather than sharp declines (Cluster 2). The most effective sadness arcs maintain emotional resilience through measured pacing, allowing for depth without overwhelming other genre elements. Interestingly, while both clusters show decreasing sadness, the gradual decline performs better than the steep drop, suggesting audiences prefer emotional resolution that feels earned rather than rushed.


Disgust, particularly important in Fantasy/Sci-Fi, works best with steady, controlled progression (Cluster 1) rather than irregular spikes (Cluster 3). This suggests that audiences need time to process unfamiliar or challenging elements, with measured introduction proving more effective than sudden exposure.

Surprise effectiveness, especially in horror, depends on maintaining consistent mid-level arousal with regular small variations (Cluster 5) rather than declining intensity (Cluster 4). This pattern allows for effective shock moments while maintaining audience engagement.

Across all genres, the most successful emotional arcs share common characteristics: sustained engagement, gradual build-ups, multiple small peaks rather than single large ones, controlled decline phases, and emotional resilience. Failed arcs typically show rapid exhaustion, premature peaks, inconsistent intensity, sharp declines, and lack of recovery points.

This analysis suggests that successful film narratives require sophisticated emotional pacing that aligns with genre-specific storytelling needs, rather than simply maximizing emotional intensity. The patterns indicate that audiences prefer measured emotional journeys that allow for proper investment and resolution over rapid or extreme emotional shifts.




4. Cluster 4's Sadness Dominance:
- Best performer for multiple genres in Sadness (Action/Adventure, Thriller, Horror, Family/Animation)
- Psychological Framework: May represent viewers who process various genres through a "melancholic lens," finding deeper emotional resonance in seemingly dissimilar content
- Social Learning Theory: Could indicate a viewer segment that has learned to engage with diverse content through emotional rather than purely narrative processing

5. Action/Adventure Emotional Spread:
- Shows significant deltas in Anger (0.22), Fear (0.21), and Sadness (0.32)
- Cultural Context: The wide emotional range suggests successful action/adventure content must balance multiple emotional triggers to maintain engagement
- Modern Media Theory: This spread might reflect the genre's evolution from pure excitement-based content to more emotionally complex narratives

