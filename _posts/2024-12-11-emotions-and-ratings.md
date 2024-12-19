---
layout: post
title:  "Analysis between emotions and ratings"
weight: 4
date:   2024-12-11 11:08:25
categories: emotions and ratings
tags: featured
---
Background on sentiment analysis?


DO barbie style, barbie does the movie rating analysis

associate to each category an emotion
see the mean rating of movies according to their categories
if horror very low rated --- less horror films produced, smaller sample --- horror dominated by emotion fear
fear is less prevalent in continents where percentage of horror less small


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

### Does a Movie's Primary Emotion Predict How Much We'll Like It?

((Do movies with different dominant emotions have different average ratings?))

We observe how the mean ratings differ between movies classified by their dominant emotion. (clarification?)

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_per_dominant_emotion.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The analysis  reveals statistically significant differences in movie ratings across different dominant emotions. Movies dominated by sadness tend to receive the highest average ratings, followed by joy and anger. Films where fear is the dominant emotion received the lowest average ratings. Thus, a movie's dominant emotion does have a meaningful relationship with how audiences rate it.

Serious, emotionally heavy films frequently tackle complex social issues and human conditions, and so are often viewed as more "meaningful".

Repeating this same analyses for each continent separately yields some interesting observations. For Asia, films where disgusts is the dominant emotion are the group with the highest mean rating, while in North America, these films rank among the lowest mean rating. DO PLOT FOR THIS??

When breaking down this analysis by continent, only Asia and North America demonstrate statistically significant differences (as indicated by their ANOVA p-values) in how movies of different dominant emotions are rated. This statistical significance makes the contrast in their reception of disgust-dominant films especially meaningful: while Asian audiences give these films their highest average ratings, North American viewers consistently rate them among their lowest. This remarkable disparity suggests fundamental differences in how these cultures process and value this specific emotional content in cinema.

Although these findings suggest that a movie's dominant emotion does influence movie ratings, the differences are relatively modest, hinting that the emotional landscape of cinema resists such simple categorization. Therefore, we adopt a more detailed approach and delve deeper into emotional diversity, that is, to what extend multiple emotions are expressed throughout a story.


### Emotional Arcs and Success: Does a More Varied Emotional Journey Lead to Greater Success?

One hypothesis is that movies with more dynamic and varied emotional arcs have a greater ability to resonate with a wider audience, in contrast to those with a more emotionally flat or one-dimensional narrative.

To quantify "emotional diversity" in movies, we employed four distinct metrics:
1. Shannon Entropy: Measures the overall balance of emotions throughout the movie - higher values indicate a more even distribution across different emotions rather than dominance of just one or two
2. Emotion Transitions: Counts how often the dominant emotion changes, capturing the dynamic shifts in emotional tone
3. Emotion Variation: Measures the standard deviation of emotional intensities over time, showing how much emotions fluctuate
4. Unique Dominant Emotions: Simply counts how many different emotions take the lead at some point in the movie

We perform a general analysis of the ratings with the diversity metrics, and find the following correlations: 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_general_diversity.html" 
    width="100%" 
    height="425" 
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

In Europe and North America, all metrics show consistent, statistically significant positive correlations with ratings. This suggests that Western audiences tend to rate movies more favorably when they feature more diverse emotional content.

South America shows the strongest positive correlations among all continents. This indicates that South American audiences may be particularly appreciative of emotionally diverse films, with emotion transitions having the strongest impact on ratings. This likely reflects deep cultural roots in melodramatic storytelling, particularly through telenovelas. Telenovelas, which originated in Latin America, are characterized by intense emotional oscillations and dramatic transitions. 

Asia presents an interesting case where emotion transitions show the strongest correlation with ratings, while other metrics have weaker relationships. This results reflect different cultural and cinematographic traditions, as in many East Asian countries, movies maintain consistent emotional tones within genres, e.g., consistent melancholy in many dramas, which may explain the unsignificant correlation with Shannon entropy.

Oceania and Africa were excluded from this analysis as their limited sample size may affect the statistical power of it. 

### Do we really want happy endings? The numbers tell a different story

To dig deeper into this question, we classify movies according to their ending, looking at the emotions in the last timestep.

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

This analysis suggests that the relationship between ending type and audience reception is more complex than might be expected, and that successful movies don't necessarily need to have happy endings to be well-received by audiences. The impact of ending type appears to be genre-dependent.

In Drama and Romance, movies with sad endings tend to receive slightly higher ratings than those with happy endings. This might suggest that audiences appreciate emotional depth and tragic elements in these genres, perhaps viewing them as more meaningful or artistically valuable
On the other hand, Fantasy/Sci-Fi shows a reverse pattern, where happy endings rate slightly higher than sad endings. 


### How do ratings distribute across different movie categories?

This accounts for movies that belong to multiple categories, as they are counted in each category they belong to. 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_by_category.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>


Dramas have the highest mean rating, which may reflect how this genre often deals with complex human experiences and social issues, as these films often explore universal themes (family, love, loss, identity) that resonate across cultural boundaries. (connection with dramas having more sadness -- dominant emotion with highest rating!)

Horror films have the lowest mean rating, which can be attributed to the genre's polarizing nature - people tend to either love or hate horror. Additionnaly, there may exist a cultural stigma around horror as a "less serious" genre. 


### Emotion ARCS and ratings

With K-Shape clustering per emotion, find the best and worst performing cluster for each movie category per emotion. 
Analyze only the categories and emotions where Δ(best-worst) > 0.15, focusing on the most statistically significant patterns:
- Sadness: 
    - Best: Cluster 4 is the best performing cluster for Action/Adventure, Drama, Thriller, Horror and Family/Animation. This cluster represents a clear/gradual decline/decrease in sadness over time.
    - Worse: Cluster 2 is the worst performing cluster for Action/Adventure, Drama, Thriller, Family/Animation. This cluster represents a steep sadness decreade
    - Interestingly, while both clusters show decreasing sadness, the gradual decline performs better than the steep drop, suggesting audiences prefer emotional resolution that feels earned rather than rushed.
- Joy:
    - Look at  Action/Adventure, SciFi

Conclusions: while analysing Sadness, we can remark that Cluster 4 is best-performing for many categories, boasting a graudal decrease in sadness over time. Meanwhile, the worst performing tends to be Cluster 2, where there is a steep sadness decrease. This suggests movies benefit from carefully paced emotional resolution rather than quick emotional shifts, perhaps allowing for more meaningful character development. (benefit from measured emotional pacing rather than abrupt changes in emotional tone.)(suggests audiences prefer a gradual easing of emotional tension over sharp emotional drops. This aligns with the genre's need to maintain suspense and engagement throughout the narrative.")

Action/Adventure:
- Joy: (Δ: 0.15)
Cluster 1 performs best, showing a stable low-medium joy level that rises sharply at the end. This measured approach to joy suggests successful action films don't rely on constant excitement but build to a satisfying climax. Best: Cluster 1 - stable low-medium joy with sharp final rise. Worst: Cluster 3 - gradual increasing joy throughout. The contrast suggests that audiences prefer a "delayed gratification" approach over steady joy increase, reinforcing the importance of an emotionally impactful climax.


Horror: 
Worst: Cluster 5 - increasing sadness
The contrast here is particularly interesting as it suggests successful horror films don't rely on increasing sadness, perhaps focusing more on other negative emotions like fear or tension.

Key Insights from Significant Deltas (>0.15):
1. Sadness resolution appears critically important across multiple genres, with particularly strong effects in Action/Adventure (Δ: 0.32) and Fantasy/Sci-Fi (Δ: 0.31).
2. The largest emotional impacts are found in sadness patterns rather than joy patterns, suggesting audience response is more sensitive to how negative emotions are handled.
3. Fantasy/Sci-Fi shows significant deltas in both emotions, indicating it's a genre where emotional arc management is particularly crucial.
4. Action/Adventure shows significant deltas in both emotions, suggesting careful emotional pacing is key to success in this genre.
5. The consistently high deltas for Cluster 4's decreasing sadness pattern across multiple genres suggests this might be a universal principle of successful storytelling.



Example films from top 10%:
        Movie_name  Rating  anger  disgust  fear  joy  sadness  surprise
1     Blade Runner     8.1    4.0      1.0   1.0  0.0      0.0       1.0
2  Blazing Saddles     7.7    4.0      0.0   1.0  0.0      0.0       4.0
3      Blue Velvet     7.7    4.0      2.0   1.0  0.0      0.0       1.0
4     Barry Lyndon     8.1    3.0      1.0   3.0  0.0      0.0       1.0
6       Braveheart     8.3    2.0      0.0   4.0  0.0      0.0       1.0

==================================================
SUMMARY: Dominant Emotion Clusters (>30% share)
==================================================

Emotion: ANGER
Cluster 4.0: 31.2% (1036 films) . mild increase of anger , decrease a h
Example films from this cluster:
- Blade Runner (Rating: 8.1)
- Blazing Saddles (Rating: 7.7)
- Blue Velvet (Rating: 7.7)

Emotion: DISGUST
Cluster 0.0: 30.4% (1008 films)
Example films from this cluster:
- Blazing Saddles (Rating: 7.7)
- Braveheart (Rating: 8.3)
- Citizen Kane (Rating: 8.3)

Emotion: FEAR
Cluster 1.0: 33.2% (1103 films)
Example films from this cluster:
- Blade Runner (Rating: 8.1)
- Blazing Saddles (Rating: 7.7)
- Blue Velvet (Rating: 7.7)

Emotion: JOY
Cluster 0.0: 48.4% (1606 films)
Example films from this cluster:
- Blade Runner (Rating: 8.1)
- Blazing Saddles (Rating: 7.7)
- Blue Velvet (Rating: 7.7)

Emotion: SADNESS
Cluster 0.0: 39.5% (1312 films)
Example films from this cluster:
- Blade Runner (Rating: 8.1)
- Blazing Saddles (Rating: 7.7)
- Blue Velvet (Rating: 7.7)

Emotion: SURPRISE
Cluster 1.0: 48.1% (1597 films)
Example films from this cluster:
- Blade Runner (Rating: 8.1)
- Blue Velvet (Rating: 7.7)
- Barry Lyndon (Rating: 8.1)
<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/best_and_worst_clusters_general.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>