---
layout: post
title:  "Analysis between emotions and ratings"
date:   2024-12-11 11:08:25
categories: emotions and ratings
tags: featured
---
Background on sentiment analysis?

How do emotion affect movie's successes? 

To answer the myriad of following questions, and after having performed an exhaustive sentiment analysis on the film's summaries, we embark on a journey to decipher how sentiments affects a movie's success (in terms of user ratings). Having divided the movies into 20 timesteps, each with a emotion score for each of 7 emotions, we can plunge in depth in analysing how and to what extent the presence of emotions is decisive/causal/significant.

What sentiments do we seek to find in the big screens/in movies? What are the imperative emotional ingredients needed to satiate our soul's/mind's/hearts cinematographic hunger?

By calculating the mean value for each emotion across all timesteps for each movie, determining which emotion has the highest mean value and naming this the movie's dominant emotion, we can see how the mean rating differs among this classification. We then attempt to answer to the questions: "Do movies with different dominant emotions have different average ratings?"

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_per_dominant_emotion.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

As we can see from these results, and while also performing a one-way ANOVA test (result??), these findings suggest that while emotional content does influence movie ratings, the differences are relatively modest (all means are within about 0.5 points of each other). The statistical significance likely comes from the large sample size rather than large practical differences in ratings.

(Comment on results of dominant_emotion_rating and one-way ANOVA per continent? Europe not significant, NA significant - maybe due to large sample size)

Therefore, rather than attempting to classify movies according to their dominant emotion, we seek to answer a more detailed question.
(shall try to narrow down/characterise our analysis in a more detailed manner to try to find some robust results.)

Looking now at emotional variety, to what extend multiple emotions are expressed throughout a story.

Does a more varied emotional journey lead to higher ratings? Do movies with multiple emotions expressed throughout the story garner higher success?

Do movies with greater emotional diversity  attract larger audiences or have better movie ratings? What is the impact of having many emotions expressed significantly rather than having lesser dominant emotions? Do certain emotion arcs archetypes play a particularly significant role in determining a movie's success?

A possible (??) hypothesis is that movies with more varied emotional arcs resonate with a broader audience compared to those that remain emotionally flat.


To quantify "emotional diversity" in movies, we employed four distinct metrics:
1. Shannon Entropy: Measures the overall balance of emotions throughout the movie - higher values      indicate a more even distribution across different emotions rather than dominance of just one or two
2. Emotion Transitions: Counts how often the dominant emotion changes, capturing the dynamic shifts in emotional tone
3. Emotion Variation: Measures the standard deviation of emotional intensities over time, showing how much emotions fluctuate
4. Unique Dominant Emotions: Simply counts how many different emotions take the lead at some point in the movie


<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_general_diversity.html" 
    width="100%" 
    height="700" 
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

Both Europe and North America show strong and significant results, implying these audiences appreciate emotional complexity (?) and diversity. South America possesses the strongest correlation coefficient among all regions, suggesting South American audiences highly value emotional variety. Finally, Asia presents mixed results, having weaker correlations overall and suggesting different emotional preferences compared to Western regions. LITERATURE REVIEW REFERENCE?

Oceania and Africa were excluded from this analysis as their limited sample size may affect the statistical power of it. 

Cultural Implications
   - Clear distinction between Western and non-Western markets
   - Suggests different cultural preferences for emotional complexity
   - Indicates need for region-specific approach in film emotional content

We then perform a mixed effects analysis with emotional diversity, selecting a unique emotion diversity metric, the Shannon entropy. The aim is to show how emotional diversity affects ratings within each category.

The model shows a significant positive relationship between emotional diversity and ratings (coefficient = 0.643, p < 0.001). This indicates that, across all genres, higher emotional diversity tends to be associated with higher ratings

Horror shows the strongest relationship, with Action/Adventure and Thriller following closely. Family/Animation shows the weakest relationship. The strong positive coefficients across all genres suggest that emotional diversity generally enhances viewer ratings. Horror films show the strongest benefit from emotional diversity, despite having the lowest mean ratings. Family/Animation shows the weakest relationship, suggesting emotional consistency might be more important for this genre