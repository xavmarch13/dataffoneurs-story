---
layout: post
title:  "Indiana Jones and the map of movie success: following the emotional trail"
weight: 6
date:   2024-12-11 11:08:25
categories: emotions and ratings
tags: featured
image: /assets/Plots/PlotsRatings/indiana-jones-great-circle-marquee.jpg
image2: /assets/Plots/PlotsRatings/indiana-jones-great-circle-marquee.jpg
previous_post: /dataffoneurs-story/jekyll/update/2024/12/11/welcome-to-jekyll.html
---
By Dr. Henry “Indiana” Jones Jr

Ladies and gentlemen, welcome to this archeological excavation site! 

Like any good archaeological dig, we're not just looking for surface artifacts. No, we're going deeper - much deeper. We're excavating through layers of data to uncover the fundamental mysteries of what makes movies resonate with audiences. What emotional treasures do we seek in the darkness of the theater? What combinations of feelings create that perfect alchemy of high ratings?

Our expedition will take us through treacherous territory as we attempt to decode:

- The primary emotional chambers that form cinema's foundation - which ones lead to ratings gold, and which ones might be better left sealed
- The intricate dance of multiple emotions - is a varied emotional journey like a well-balanced ancient mechanism, or do audiences prefer a simpler path?
- The age-old question of happy versus sad endings - sometimes, the most valuable treasures aren't the ones that make you smile
- And perhaps most importantly, those elusive patterns of emotional flow that separate the cinematic Holy Grails from the forgotten relics

I've brought along my finest archaeological tools - statistical analysis more precise than any ancient map, emotional measuring devices that would make even the most seasoned temple guardians raise an eyebrow, and years of experience in pattern recognition that's saved my life more times than I can count.

So grab your statistical tools and emotional compasses, folks. We're about to venture into the heart of cinema's emotional temple, and I have a feeling this might be our most revealing expedition yet...


Let's start our expedition by examining the basic terrain - the different genres that make up our cinematic landscape...

###  The quest for genre excellence
<br />
You know, after decades of exploring ancient ruins, I've learned that some treasures are universally valued while others... well, let's just say they're an acquired taste. The same seems to hold true for movie categories.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_by_category.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Take Drama, for instance - sitting pretty at the top. It reminds me of those universal artifacts we find across different civilizations - the ones that tell stories of love, loss, family, and identity. Just like how a mother's tears look the same whether you're in the jungles of South America or the deserts of Egypt, these fundamental human experiences resonate across all cultural boundaries.

Romance and Family/Animation follow close behind, like trusted companions on an expedition. Comedy and Thrillers maintain a respectable middle ground.

But Horror... *chuckles* 
With the lowest mean rating, it's like that cursed idol that half the people want to study and the other half want to leave buried in the temple. People either embrace it like a long-lost relic or avoid it like a booby trap.

The numbers tell us something I've learned in my adventures - the most valuable treasures aren't always the ones that make you jump with excitement. Sometimes, they're the ones that make you sit down and contemplate the deeper mysteries of human existence.

Now that we've mapped out the genre territory, let's venture deeper into the emotional chambers of these cinematic temples. What we found here might surprise even the most seasoned adventurer...

### Field notes on fundamental feelings
<br />
We've uncovered something fascinating.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/mean_rating_per_dominant_emotion.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>


Movies where sadness is the dominant emotion - and believe me, I've had my share of those moments in dark temples - actually score the highest ratings! They're followed closely by films dominated by joy, and then those powered by anger.

But why do sad movies take the lead? Well, these films usually tackle deeper human experiences. They're like ancient scrolls that reveal profound truths about the human condition - not just entertainment, but real meaning.
Remember how Drama had the highest mean ratings? Well, it's no coincidence then that sadness scores the highest in dominant emotions, as Drama is the genre that most often carries that emotional weight.You saw that with my old friends Neo! The cluster 4 is the one with the most sadness and also the one with the biggest proportion of Drama movies... It's like finding matching pieces of an ancient puzzle.

Now, here's where it gets interesting - films where fear leads the emotional charge actually received the lowest ratings. Apparently, audiences prefer their movies to dig deeper into other emotional territories.

*Pulls out a continental map*

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/figasiana.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

But the most remarkable findings came from our continental excavation. Out of all the regions we studied, only North America and Asia showed statistically significant patterns - like finding two distinct civilizations with clear, measurable differences in their artifact preferences. 
The most striking contrast between these two cultures? Their reaction to disgust-dominant films. In Asia, these productions receive their highest average ratings, suggesting a unique cultural appreciation for this type of emotional storytelling. Meanwhile, North American audiences consistently rate these same types of films among their lowest - it's like discovering two ancient cultures had completely opposite uses for the same artifact.

However, just like how you can't judge a tomb by its entrance, we can't fully evaluate a movie just by its dominant emotion. The differences we're seeing here are like finding subtle variations in ancient pottery - meaningful, but not the whole story.

That's why we need to dig deeper, folks. Just as one artifact doesn't tell us everything about an ancient civilization, one emotion doesn't tell us everything about a movie. We need to look at how these emotions interact and flow throughout the story...

### The kingdom of emotional diversity
<br />
You know, after decades of chasing ancient artifacts, I've started asking myself a different kind of question: What makes a journey truly memorable? Is it the constant shifts between terror and triumph, like when you're running from a rolling boulder one minute and discovering a priceless artifact the next? Or is it maintaining a steady course, like following a single ancient map to its destination? 

After deep reflection, I've concluded that the most valuable journeys often have multiple layers, just like Stanley Kubrick suggested. 

*Pulls out Kubrick's quote from a worn leather pouch*

> "A film is--or should be--more like music than like fiction. It should be a progression of moods and feelings."

Wise words from Kubrick - reminds me of navigating through temple chambers, each room holding a different emotional trap or reward.

Now, folks, we've developed four sophisticated measuring tools:

First, we've got the **Shannon entropy** measure - think of it like examining a tomb's contents. Are all the treasures diverse, or is it just filled with one type of artifact? 

Then there's the **emotion transitions** counter - similar to counting the number of times I've had to switch from running to fighting to puzzle-solving in one adventure. 

**Emotion variation** measures how intensely emotions fluctuate over time. Think of it as measuring the depth of different chambers in a cave - some might be shallow, others deeper than expected. It tells us if a movie stays emotionally level or takes us on a rollercoaster ride worthy of the mine cart chase in Temple of... well, you know the one.

And finally, **unique dominant emotions** is most straightforward of our tools, like my trusty whip. It simply counts how many different emotions take the lead throughout the film. It's like counting how many different types of challenges you face in an adventure - the more variety, the more interesting the journey.

We can now perform a correlation between these four emotional diversity metrics and ratings: 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_general_diversity.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>


The data shows something fascinating - like finding a small positive inscription on an ancient tablet. It shows a positive connection, meaning movies with more emotional variety do tend to get better ratings, but this correlation is as subtle as the markings on the Staff of Ra - significant if you know what you're looking for, but easy to miss if you're not paying attention.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/correlation_continent_diversity.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Now, this is where it gets interesting - like finding different archaeological traditions across continents. In Europe and North America, they appreciate emotional diversity like they appreciate their museums - consistently and significantly. 

South America shows the strongest appreciation for emotional transitions - stronger than my grip when hanging from a cliff! This reminds me of their telenovela tradition - those melodramatic stories have more twists and turns than the Venetian catacombs.

And Asia - now there's an interesting case. They value emotional transitions highly, but other metrics? Not so much. It's like how different cultures build different types of temples - some prefer consistency, others variety.<br />
You see, in many East Asian cinematographic traditions, movies often maintain a consistent emotional tone within their genres. Take their dramas, for instance - they embrace melancholy with the same dedication that I pursue archaeological truth. It's not about jumping between emotions like a Western action sequence; it's about diving deep into a single emotional current and staying there, like exploring the depths of an underground temple.
That's not a flaw in their storytelling - it's a feature! It's like how some of the most precious artifacts I've found weren't decorated with a thousand different patterns, but rather perfected in their singular purpose.

As for Oceania and Africa, well, sometimes you need more artifacts before you can make solid conclusions about an ancient civilization. We'll need more data from these regions before we can make any definitive statements.

What we've discovered here is that emotional diversity in movies is like a well-balanced ancient artifact - it contributes to its value, but it's not the only thing that makes it precious. Sometimes it's not about finding the Holy Grail, but understanding how different cultures value different aspects of storytelling.
These different storytelling traditions that have evolved over thousands of years, each as valid as the next. Just like how every ancient civilization had their own unique way of recording their history.

Speaking of emotional journeys, I've encountered a particularly fascinating artifact that might challenge everything we think we know about happy endings...

### The temple of dramatic conclusions: why happy endings aren't always the greatest treasure
<br />
You know, in all my years of archaeology and adventures, I've rarely come across a quote that rings as true as what Fyodor Dostoevsky once wrote:

> "Man only likes to count his troubles; he doesn’t calculate his happiness."

Reminds me of the time I was counting my bruises after that run-in with the Temple of Doom, instead of celebrating the fact I'd made it out alive!

And speaking of human nature's peculiar relationship with suffering, our excavation of movie data has revealed some fascinating patterns that would make old Fyodor nod in agreement. Let me show you what we've unearthed.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/distribution_by_category_and_ending.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

In the grand museum of cinema, Drama dominates the sad endings section like a colossal statue - commanding 41.4% of all sad-ending films, compared to just 29% of happy ones. Romance stories, much like the cursed artifacts I've encountered, show up consistently in both happy and sad territories, proving that love stories can break hearts just as effectively as they can mend them.


<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/average_ratings_by_category_and_ending.html" 
    width="100%" 
    height="700" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

In both Drama and Romance, audiences actually rate the sad endings slightly higher than the happy ones. It's as if we're drawn to emotional pain like moths to an ancient ceremonial flame!

The Fantasy and Sci-Fi genres, however, buck this trend like a stubborn mule in the Himalayas. These audiences prefer their endings happy, perhaps because after journeying through strange new worlds, they want the satisfaction of a triumphant return - something I can certainly relate to after my expeditions!

What we're seeing here validates Dostoevsky's observation. We might say we want happy endings, but just like how I keep going back to dangerous archaeological sites, audiences seem to find something particularly compelling about stories that end in tears rather than cheers - at least in certain genres.

*Puts notebook away and straightens hat*

Now, for the crown jewel of our expedition - the detailed patterns that emerge when we examine these emotional journeys under our finest archaeological instruments...

### Raiders of the lost story shapes: decoding the emotional DNA of successful films 
<br />
Well folks, after years of exploring ancient temples, I've stumbled upon something even more intricate - the emotional architecture of modern cinema. And let me tell you, these patterns are as complex as any maze I've navigated.

*Unrolls the emotional k-shape clustering data manuscript*

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/best_and_worst_clusters_general.html" 
    width="100%" 
    height="1400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

The most remarkable discovery is cluster 1 for joy - it's like finding the Holy Grail of emotional patterns! This cluster emerges as the champion across six different genres, from Action/Adventure to Horror. It's clearly got something special in its DNA that resonates with audiences.

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_drama_movie_joy_cluster1.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Looking at the time evolution graphs, we can see why - cluster 1 maintains a steady emotional intensity without wild fluctuations, much like navigating a careful path through a booby-trapped temple. 
"The First Grader" demonstrates this - it's structured like a classic hero's journey! The emotional shape forms a perfect dramatic 'U', starting with an initial burst of joy, taking us through a long middle journey of anticipation, and finally rewarding us with a triumphant emotional crescendo at the end. This is storytelling architecture at its finest!

For fear, cluster 6 appears to be our villain - it consistently underperforms across eight different genres! In the evolution graphs, we can see it peaks early but then drops off dramatically, like a boulder rolling down behind us in a chase scene.

Let's take a closer look at this worst-performing fear cluster: 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_thriller_fear_cluster6.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>


An interesting artifact appears in the surprise category - the best-performing cluster 3 shows a special affinity for both Fantasy/Sci-Fi and Family/Animation. Looking at its evolutionary pattern: 

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_family_surprise_cluster3.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

"The Band Concert"'s surprise pattern shows masterful restraint, with small, carefully placed peaks like stepping stones across a stream. Instead of trying to overwhelm the audience, it creates a gentle rhythm of small discoveries.

Ah, these new discoveries add fascinating layers to our emotional archaeology! Let me add my field notes:

For the Fantasy/Sci-Fi disgust emotion in cluster 3, we have the "Bedhead" movie, which is the case of a worst-performing cluster:

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_fantasy_disgust_cluster3.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

 And what a peculiar specimen it is!  The shape is remarkable - it maintains an almost perfectly flat high plateau for the first 6-7 timesteps, like a suspended moment of tension. Then comes the dramatic part - it doesn't just decline, it practically falls off a cliff between timesteps 7 and 10. This extreme pattern explains why this cluster performs poorly - it's like building up too much tension without proper release. No wonder the audiences didn't connect with it!


Now, for the Action/Adventure sadness in Cluster 4, we have "The Secret Invasion", an example of a best-performing cluster for this emotion:

<iframe src="{{ site.baseurl }}/assets/Plots/PlotsRatings/fig_action_sadness_cluster4.html" 
    width="100%" 
    height="400" 
    frameborder="0" 
    scrolling="no" 
    style="overflow: hidden; min-width: 800px;">
</iframe>

Instead of sharp drops or plateaus, we see a gently undulating line with multiple small peaks and valleys, almost like a calm ocean wave. The key feature is its gradual rise to a subtle double peak around its middle, followed by a smooth descent. It's like finding the perfect balance in an ancient scale - enough emotional weight to give meaning to the action, but not so much that it overwhelms the adventure. This controlled approach to sadness allows the action elements to shine through while maintaining emotional depth.

Now, our cautionary tales: "Nella stretta morsa del ragno" and "Bedhead", both examples of worst-performing clusters for their respective emotions, show us what happens when emotional architecture goes awry. Both follow a similar problematic pattern - they're like inverted pyramids, unstable by design. In "Nella stretta morsa," the fear pattern creates an unsustainable plateau that collapses, while "Bedhead's" disgust pattern maintains an unnaturally flat high level before its dramatic plummet. These shapes lack the dynamic flow that audiences connect with.

*Packs up surveying equipment*

These examples perfectly illustrate why some emotional patterns become treasured artifacts while others end up as cautionary tales in our cinematic archaeology. The key seems to be in the balance and timing of emotional intensity, much like knowing exactly when to swap a bag of sand for a golden idol!


Now that's what I call an adventure in emotional archaeology! These patterns could be worth a fortune to the right filmmaker... if they can decode their secrets.

### Time to say goodbye!
<br />
Well, folks, we've traveled through every chamber of this emotional temple, from the broad halls of genre analysis to the intricate patterns of emotional clustering. Like any good archaeological expedition, we've discovered that the real treasure isn't in any single finding, but in how all these pieces fit together to tell us a greater story about human nature and storytelling.

And remember - these patterns and emotional artifacts don't belong locked away in some dusty academic journal. They belong in the hands of storytellers who can use them to create the next generation of cinematic treasures!




