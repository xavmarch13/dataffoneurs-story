---
layout: post
title:  "Analysis between emotions and ratings"
weight: 7
date:   2024-12-11 11:08:25
categories: emotions and ratings
tags: featured
---
Background on sentiment analysis?
The essence of cinema lies in its ability to evoke and explore the depths of human emotion, serving as a mirror to our shared experiences and inner lives. Emotions in movies transcend mere storytelling, becoming a universal language that connects us to characters, moments, and each other. They reveal the complexities of existence, illuminating joy, sorrow, love, and conflict in ways that words alone cannot. 

In this section, we embark on a journey to decipher/unravel the intricate relationship between emotions and a movie's success, focusing specifically on how they influence viewer ratings. Delving deeper, we seek to uncover not only the presence of emotions but also their dynamics — exploring how these emotional elements contribute to shaping audience reception and appraisal.
Through this lens, we aim to illuminate the emotional alchemy that lies at the heart of cinematic triumph.


In the following we will attempt to provide an intuition to the myriad of questions such as:
- What emotions do we seek to experience on the big screen? What are the essential emotional ingredients required to satisfy our soul’s cinematic hunger?
- Does a more varied emotional journey lead to higher ratings? Do movies with multiple emotions expressed throughout the story garner higher success?
- MORE !!!!

## The Influence of Emotions in a Movie's Success

<br />

### Do movies with different dominant emotions have different average ratings?

We observe how the mean ratings differ between movies classified by their dominant emotion. (clarification?)

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_per_dominant_emotion.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The analysis, including a one-way ANOVA test, reveals statistically significant differences in movie ratings across different dominant emotions (F = 19.945, p < 0.001). Movies dominated by sadness tend to receive the highest average ratings, followed by joy and anger. Films where fear is the dominant emotion received the lowest average ratings. Thus, a movie's dominant emotion does have a meaningful relationship with how audiences rate it.

(! do more in detail: Using sampling techniques to balance the dataset)
(Comment on results of dominant_emotion_rating and one-way ANOVA per continent? Europe not significant, NA significant - maybe due to large sample size)

Serious, emotionally heavy films frequently tackle complex social issues and human conditions, and so are often viewed as more "meaningful".

Although these findings suggest that a movie's dominant emotion does influence movie ratings, the differences are relatively modest, hinting that the emotional landscape of cinema resists such simple categorization. Therefore, we adopt a more detailed approach and delve deeper into emotional diversity, that is, to what extend multiple emotions are expressed throughout a story.

### Emotional Arcs and Success: Does a More Varied Emotional Journey Lead to Greater Success?


One hypothesis is that movies with more dynamic and varied emotional arcs have a greater ability to resonate with a wider audience, in contrast to those with a more emotionally flat or one-dimensional narrative.

To quantify "emotional diversity" in movies, we employed four distinct metrics:
1. Shannon Entropy: Measures the overall balance of emotions throughout the movie - higher values indicate a more even distribution across different emotions rather than dominance of just one or two
2. Emotion Transitions: Counts how often the dominant emotion changes, capturing the dynamic shifts in emotional tone
3. Emotion Variation: Measures the standard deviation of emotional intensities over time, showing how much emotions fluctuate
4. Unique Dominant Emotions: Simply counts how many different emotions take the lead at some point in the movie


<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_general_diversity.html" 
    width="100%" 
    height="425" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

We can observe that movies with more diverse and dynamic emotional content tend to receive slightly higher ratings, supporting the hypothesis that emotional variety resonates with audiences. However, the relatively small correlation coefficients suggest that while emotional diversity does play a role in audience reception, it's likely just one of many factors that influence overall movie ratings.

We decide to do this analysis by continental regions, to see if we can witness any stronger correlations that may indicate difference preferences. 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_continent_diversity.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The relationship between emotional diversity and movie ratings shows interesting geographical variations. 

In Europe and North America, all metrics show consistent, statistically significant positive correlations with ratings. This suggests that Western audiences tend to rate movies more favorably when they feature more diverse emotional content.

South America shows the strongest positive correlations among all continents. This indicates that South American audiences may be particularly appreciative of emotionally diverse films, with emotion transitions having the strongest impact on ratings. This likely reflects deep cultural roots in melodramatic storytelling, particularly through telenovelas. Telenovelas, which originated in Latin America, are characterized by intense emotional oscillations and dramatic transitions. 

Asia presents an interesting case where emotion transitions show the strongest correlation with ratings, while other metrics have weaker relationships. This results reflect different cultural and cinematographic traditions, as in many East Asian countries, movies maintain consistent emotional tones within genres, e.g., consistent melancholy in many dramas, which may explain the unsignificant correlation with Shannon entropy.

Oceania and Africa were excluded from this analysis as their limited sample size may affect the statistical power of it. 

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

