---
layout: post
title:  "2. Clustering Analysis!"
weight: 10
categories: mediator feature
image: /assets/article_images/2014-11-30-mediator_features/night-track.JPG
image2: /assets/article_images/2014-11-30-mediator_features/night-track-mobile.JPG
---
## Can we classify films by anything other than genre?
Can emotions help us see if different trends exist? Can we categories film by their emotion et not by their genre?
We'll find out in this section.
<div class="row">
    <div class="col-md-6">
        <iframe src="{{ site.baseurl }}/assets/plot/cluster/pca_kmeans.html" 
                style="width: 100%; height: 900px; border: none;"></iframe>
    </div>
    <div class="col-md-6">
        <iframe src="{{ site.baseurl }}/assets/plot/cluster/barplot_highest_emotions.html" 
                style="width: 100%; height: 900px; border: none;"></iframe>
    </div>
</div>


<p> 
    Comme nous pouvons le voir avec le graphe suivant, chaque cluster représente la catégorie de film qui contient le plus d'une certaine émotion. 
    Par exemple, le cluster 1 représente les films qui ont le plus de <em>anger</em>, le cluster 2 la catégorie de film qui ont le plus de <em>joy</em>, etc.
</p>
On peut voir que par rapport à la distribution global des genres, les films d'Action et les Thrillers sont surreprésenté. Dans les films ou le Joy est le plus présent, on a une surreprésentation des films Drama et Romance et Comedy tandis que les thrillers et les films d'horreurs n'ont pas beaucoup de joy visiblement. La comedy et les animations sont sur-représenté dans les films avec beaucoup de surprise. Comme pour le cluster 2, les films avec beaucoup de sadness sont très principalement des films de Drama et de ROmance. Dans le cluster 5, le cluster des films avec le plus de fear, c'est les Thriller et les films d'horreur qui sont bien présents. Dans les films avec veaucoup de dégout, c'est principalement les films d'horeurs. et pour le dernier cluster, c'est principalement la comedy, le family/animation et le Fantasy-SCI.
PTETRE FAUDRAIT DIVISER CHAQUE VALEUR PAR SA PROPORTION GLOBAL POUR AVOIR UN NOMBRE +- grand que 1
<iframe src="{{ site.baseurl }}/assets/plot/cluster/repartition_overall_and_cluster.html" width="100%" height="700" frameborder="0"></iframe>  
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_per_category.html" width="100%" height="1600" frameborder="0"></iframe>  
# Analysis of Cluster Distribution by Genre and Emotions

## Cluster 1 - Anger
- **Highest proportion of anger**: *30.3% in Action/Adventure*, *26.5% in Thriller*.  
- **Analysis**:  
  Action and adventure films generate anger primarily through themes of conflict, rivalry, and injustice. Physical confrontations, chases, and revenge-driven plots are hallmarks of the genre, evoking strong emotional reactions.  
  In dramas, anger arises from frustration caused by unjust or tragic situations faced by the characters. This often reflects the audience's identification with societal, familial, or personal conflicts.
  ### Example: 
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_1.html" width="100%" height="700" frameborder="0"></iframe>  

## Cluster 2 - Joy
- **Highest proportion of joy**: *13.7% in Comedy*, *20% in Romance*.  
- **Analysis**:  
  While comedies aim to evoke joy, the proportion remains relatively low (13.7%), likely because humor is often intertwined with surprise or neutral elements, creating a mixed emotional experience.  
  In romances, joy is more prominent (20%) as these films focus on moments of happiness, fulfilled love, and positive resolutions of relational conflicts.

<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_2.html" width="100%" height="700" frameborder="0"></iframe>  

## Cluster 3 - Surprise
- **Highest proportion of surprise**: *11.3% in Family/Animation*, *9.89% in Comedy*.  
- **Analysis**:  
  Family/animation and fantasy/science fiction films thrive on imaginative worlds, unexpected plot twists, and visually spectacular elements. These genres cultivate curiosity and wonder, which are core components of surprise.  
  Plot reversals and magical or futuristic scenarios encourage viewers to explore new possibilities, evoking both surprise and fascination.
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_3.html" width="100%" height="700" frameborder="0"></iframe>  


## Cluster 4 - Sadness
- **Highest proportion of sadness**: *20.7% in Romance*, *19.5% in Drama*.  
- **Analysis**:  
  Dramas delve into emotions of loss, hardship, and human sacrifice, often presenting realistic emotional conflicts that evoke authentic sadness in viewers.  
  Romances, while generating joy, also explore themes of heartbreak, unfulfilled love, or emotional dilemmas, leading to sadness when relational conflicts remain unresolved.
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_4.html" width="100%" height="700" frameborder="0"></iframe>  


## Cluster 5 - Fear
- **Highest proportion of fear**: *29.7% in Horror*, *20.2% in Thriller*, *19.2% in Fantasy/Sci-Fi*.  
- **Analysis**:  
  Horror films evoke primal fear and anxiety through themes of survival, imminent danger, or supernatural elements. Psychological theories suggest fear triggers strong physiological responses (adrenaline and muscle tension), enhancing audience immersion.  
  Thrillers induce a more cognitive form of fear, relying on suspense, hidden threats, and plot twists to maintain a state of tension and unease.
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_5.html" width="100%" height="700" frameborder="0"></iframe>  

## Cluster 6 - Disgust
- **Highest proportion of disgust**: *30.3% in Horror*.  
- **Analysis**:  
  Horror films often elicit disgust through graphic, violent, or disturbing imagery. Disgust is tied to instinctual reactions of repulsion and self-preservation, amplifying the sensory impact of the viewing experience.
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_6.html" width="100%" height="700" frameborder="0"></iframe>  

## Cluster 7 - Neutral
- **Highest proportion of neutrality**: *40.5% in Family/Animation*, *35.5% in Fantasy/Sci-Fi*.  
- **Analysis**:  
  Family and comedy films tend to avoid extreme emotions, opting for light, balanced narratives that are accessible to broader audiences. This emotional neutrality reflects a desire to provide positive experiences without overwhelming viewers.
<iframe src="{{ site.baseurl }}/assets/plot/cluster/cluster_7.html" width="100%" height="700" frameborder="0"></iframe>  

---

### **General Conclusion**

The analysis of film clusters and their dominant emotions reveals a strong correlation between film genres and emotional experiences, aligning closely with established emotion theories:

- **Negative Emotions** (anger, sadness, fear, disgust):  
  - These emotions are most prevalent in genres like *drama*, *thriller*, and *horror*, which frequently explore themes of tension, loss, and threat.  
  - Such emotions provide a form of catharsis, allowing audiences to process and immerse themselves in intense and challenging narratives.

- **Positive Emotions** (joy, surprise):  
  - Positive emotions dominate in *comedy*, *romance*, and *family/animation* genres, where the focus is on creating lighthearted, entertaining, and awe-inspiring experiences.  
  - Optimistic storytelling, humorous elements, and visually engaging content stimulate joy and surprise, making these genres accessible and uplifting.

- **Emotional Neutrality**:  
  - Emotional neutrality is primarily associated with *family* and *comedy* films, which aim for emotional balance to cater to a broader audience.  
  - This neutrality reflects a deliberate storytelling approach that avoids extreme emotions, prioritizing accessible narratives and enjoyable experiences.

---

### **Summary of Observations**  
The clustering analysis underscores the emotional "specialization" of film genres:  

1. **Horror** and **thrillers** excel in evoking primal emotions like fear and disgust, creating suspenseful, high-stakes viewing experiences.  
2. **Drama** and **romance** primarily explore sadness and anger, often through realistic depictions of personal or societal struggles.  
3. **Comedy** and **family/animation** films evoke joy and emotional neutrality, offering escapism and lighthearted entertainment.  
4. **Fantasy/Sci-Fi** genres highlight surprise and neutrality, as they immerse viewers in imaginative and visually spectacular worlds.  

---

