---
layout: post
title:  "Presentation of the dataset!"
weight: 1
categories: mediator feature
image: /assets/images/jimmy_3.webp
image2: /assets/images/jimmy_3.webp
next_post: /dataffoneurs-story/data analysis/sentiment analysis/movies/2024/12/11/how-to-get-emotions.html
---
# 🎥 *Ladies and gentlemen, please welcome... the CMU Movie Summary Corpus dataset!* 🎤

**Jimmy Fallon enters, applause erupts**  
"Alright, folks, you’re in for a real treat tonight! This isn’t just any regular guest. This is a STAR. A true legend of the cinematic universe. Please give a warm Late Night welcome to... the **CMU Movie Summary Corpus Dataset**!"

---

### *The dataset takes the stage*  
**The spotlight shines on the dataset, which speaks in a confident tone**:  
"Thank you, Jimmy, and hello, everyone! Let me introduce myself. I’m the **CMU Movie Summary Corpus Dataset**, and let me tell you, I’ve got RANGE.  

- I’ve been collecting stories since **1893**, spanning over a century of cinema!  
- I hold **34,342 movie plot summaries**, packed with all the metadata you can imagine.  
- My genres? Oh, I’ve got EVERYTHING: Western, Crime, Romance, Animation—you name it, I’ve got it. Some movies couldn’t even pick just one, so they’re rocking multiple genres.  

Here’s a quick peek at my *Top 100 Genre Distribution*. It’s like the Golden Globes, but for movie categories:  

<iframe src="{{ site.baseurl }}/assets/plot/dataset_presentation/distribution_top_100_genre.html" width="100%" height="600" frameborder="0"></iframe>  

Thank you, thank you! You’re too kind. Now, looking at my Top 100 Genre Distribution, you might think, 'Wow, this dataset really has its act together.' And you’d be right! But let me tell you, Jimmy, the road to this glamorous distribution wasn’t as straightforward as it seems. You see, I used to be a bit of a mess—genres everywhere, with movies claiming to belong to 20 different categories at once! It was chaos.

So, what did we do? We rolled up our sleeves, put on our thinking caps, and mapped similar genres together. Cyberpunk and Alien invasion? Now neatly tucked under Fantasy/Sci-Fi. Zombie Film and Monster movie? Safely home in Horror. And voilà! We went from a cluttered chaos of hundreds of genres to a sleek, streamlined list that tells a clear story.

It’s like taking a scattered script and turning it into a blockbuster screenplay. Now, when you look at my genre distribution, you’re not just seeing data—you’re seeing a masterpiece of organization. Less confusion, more impact. And trust me, Jimmy, I’ve never looked better."

<iframe src="{{ site.baseurl }}/assets/plot/general_emotions/genre_mapping_for_action_adventure_category.html" width="100%" height="850" frameborder="0" style="border-left: 150px solid white;"></iframe>  

and this is how I looked after mapping genres together:
<iframe src="{{ site.baseurl }}/assets/plot/dataset_presentation/distribution_movie_genre_after_merge.html" width="100%" height="850" frameborder="0" style="border-left: 100px solid white;"></iframe>  

---

### *Jimmy jumps in*  
"Wow, incredible! But that’s not all, is it? You’re global, right? You’re everywhere!"  

**Dataset chuckles confidently**:  
"Oh, you bet. Movies from all over the world, Jimmy. And I’ve been keeping track of their release dates too. Sure, we’ve got a bias toward the West and more recent films—Hollywood does love to dominate—but let’s not forget the hidden gems from every corner of the globe. Check this out:  

<iframe src="{{ site.baseurl }}/assets/plot/dataset_presentation/movie_where_and_when_subplots.html" width="100%" height="700" frameborder="0" style="border-left: 80px solid white;"></iframe>  

What can I say? I’m a global phenomenon."  

---

### *When the dataset needed a boost*  
**Jimmy leans in, curious**:  
"Alright, but come on, every star has had their struggles. What’s the behind-the-scenes story? Was it all smooth sailing?"  

**Dataset sighs**:  
"Well, not exactly. Like every great story, mine had its challenges. Some of my movie summaries were... let’s just say, a little *thin*. Missing details, way too short, or just plain incomplete. So, we went out there, rolled up our sleeves, and *scraped* the data we needed to fill in the gaps.  
<iframe src="{{ site.baseurl }}/assets/plot/dataset_presentation/summary_lengths_comparison.html" width="100%" height="800" frameborder="0" scrolling="no"></iframe>  
<iframe src="{{ site.baseurl }}/assets/plot/dataset_presentation/missing_values_summary.html" width="100%" height="750" frameborder="0"></iframe>  
And Jimmy, that’s not all! We didn’t stop at summaries. Oh no, we went the extra mile and scraped **movie ratings** too. Now, I’m not just a storyteller—I’m a full-fledged movie critic. With this extra data, I’ve never looked better! You can see this histogram of the main ratings of the dataset right below!"  
<iframe src="{{ site.baseurl }}/assets/plot/dataset_presentation/hist_ratings.html" width="110%" height="520" frameborder="0"></iframe>  

---


### *Jimmy’s big reveal*  
"Alright, alright, let’s get real. This dataset isn’t just sitting in some library, folks. No, this dataset is a STAR. You’ve seen it in the biggest blockbusters:  

- **Oppenheimer: The science behind the scenes**  
    *Oppenheimer discovers sentiment analysis*

- **Matrix: Emotions reloaded**  
    *Neo's Journey Through Emotion: Uncovering Patterns in Film Sentiment*

- **Babylon: Cinema in its purest form**  
    *Babylon and the emotional evolution of cinema: how sound, color, and history redefined storytelling*

- **Indiana Jones: Archaeology of cinema history**  
    *Indiana Jones and the map of movie success: following the emotional trail*

And tonight, we’re going to dive into the dataset’s career. What made it a star? How did it land these big roles? And what’s next? Stick around to find out—it’s going to be one epic Late Night deep dive!"  

**Audience cheers as the dataset waves confidently. The stage is set for a full exploration of its cinematic journey.**  