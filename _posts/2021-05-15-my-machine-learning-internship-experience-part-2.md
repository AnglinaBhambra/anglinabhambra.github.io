---
title: My Machine Learning Internship Experience - Part 2
tags:
    - Internship
    - Machine Learning
excerpt: A round-up of the projects I was involved in, free valuable resources I used, and what I'm up to now. Read this article if you're about to embark on your journey into Machine Learning.
---

![Perspective](/images/anika-huizinga-unsplash.jpg)
Photo by [**Anika Huizinga on Unsplash**](https://unsplash.com/@iam_anih)

In my previous posts, I spoke about:  
⇒ [Part 0](https://anglinabhambra.github.io/how-i-became-a-machine-learning-engineer/) - My experience prior to my internship.  
⇒ [Part 1](https://anglinabhambra.github.io/my-machine-learning-internship-experience-part-1/) - My first week and some of the challenges thereafter.  

## TL;DR
- You don't need to be an expert on any one topic, especially when juggling multiple projects. Get good systems in place to fill in your knowledge gaps.
- Here is a short summary of my most notable tips for getting a good system in place:  
  → Make time to learn each day (Check out "Valuable Resources" below).  
  → Solidify an approach to obtaining a basic understanding of any topic.  
  → Approach projects with architecture diagrams that you can iterate on.  

----------------------------------------------------------------------------

## Projects 📝
I was mainly involved in the first phases of two projects. One was a Horizon 2020 (H2020) project, and the other was an Innovate UK project. H2020 is the biggest EU Research and Innovation programme ever. Innovate UK is part of UK Research and Innovation, a non-departmental public body funded by a grant-in-aid from the UK government.

### H2020 - HumMingBird
The aim of [HumMingBird](https://hummingbird-h2020.eu/) (it's still ongoing) is to better understand changing migration flows. My company's contribution was split into 4 sub-products, where my team's sub-product was a drought mapping system for the Horn of Africa. The work and research I did, contributed to producing the first iteration of this sub-product.

The first thing I had to do was to efficiently understand how to use satellite data to map drought in specific regions. This was a daunting task because I had very minimal experience **reading academic papers**. Embarrassing to admit, I faced my fears and asked for help. My manager walked me through the basics, then shared this [awesome article](https://towardsdatascience.com/how-you-should-read-research-papers-according-to-andrew-ng-stanford-deep-learning-lectures-98ecbd3ccfb3) on "How You Should Read Research Papers".

My colleague started building out the pipelines to implement some of the ideas that we had come up with, so I attempted **testing the pipelines using PyTests**. I definitely should have tried Unit Testing first, but I had come across a great tutorial on Twitch (mentioned below in "Valuable Resources") that explained how to use PyTests in an easy-to-understand way.

I also **created an internal app using streamlit** to keep all of the teams (sub-products) on the same page. One of my colleagues added a super informative and succinct literature review incredibly quickly to the app, which gave everyone a high-level understanding of the project and useful background information.

I also learnt how to **label and preprocess satellite data** with [QGIS](https://qgis.org/en/site/), [SNAP](https://step.esa.int/main/toolboxes/snap/), and [Airflow](http://airflow.apache.org/). Although I spent a limited amount of time using these tools, it was great to get exposure to working with them. I also helped my colleague record internal "how-to" videos, to help some of my colleagues use these tools too.

### Innovate UK - SBRI
In short, this project was about automating survey processing for railway structure gauging. To learn more about the project and what SBRI is, check out these links:
- https://www.gov.uk/government/collections/sbri-the-small-business-research-initiative
- [Network Rail & Innovate UK Railways SBRI](https://www.youtube.com/watch?v=5GUmVRWKZ2w)

During my first couple of weeks, my colleague and manager were writing the bulk of this proposal. I had only scratched the surface of understanding what [point clouds](https://info.vercator.com/blog/what-are-point-clouds-5-easy-facts-that-explain-point-clouds) were, so when I was asked to **contribute to the proposal** I felt like a HUGE imposter. I was also asked to put together a **high-level architecture diagram**, which honestly would have been comical if you saw what I put together. This was definitely a skill that I had improved. After a long period of delays, we found out we made it through to Phase 1.

Phase 1 took place during the last 3 months of my internship. To get myself to better understand the scope of the project and the data, my manager suggested that I read around the subject and **find open-source datasets to practice with**. I was also learning a lot from my colleagues through participating in code reviews. For example, **repeating a task back in my own words** to make sure I fully understand what I'm supposed to be doing.

I **created a labelling app using streamlit** that enabled human feedback in the ML algorithm loop. I worked with messy point cloud legacy data, my colleagues' code and also integrated [PyDeck](https://deckgl.readthedocs.io/en/latest/) into the app. Using the [streamlit gallery](https://awesome-streamlit.org/) I was able to some HTML and CSS too.

----------------------------------------------------------------------------

## Valuable Resources 📚
My favourite section! When figuring out your learning path, it is very easy to get overloaded with information or to feel like you're not learning anything because one resource doesn't work for you. The following list of MOOCs, YouTube channels, Twitch channels and Meetup groups are what worked best for me and what I still continue to use.

**MOOCS**. I can recommend 3 MOOCS that were most helpful for me.
1. [Copernicus](https://www.copernicus.eu/en/opportunities/education/copernicus-mooc) is the EU's Earth observation programme that offers information services drawn from satellite data.
2. [0toGANS](https://jovian.ai/learn/deep-learning-with-pytorch-zero-to-gans) by Jovian.ai. This was hands down, the best introduction to Deep Learning Course I have come across. I actually re-took this course once my internship finished.
3. [Fast.ai](https://www.fast.ai/). I learnt about web scraping and even built an image classifier. Although fast.ai welcomes beginners, 0toGANS was a much better introductory resource for me.

**YOUTUBE**. There are so many more channels that I could recommend, but I'll stick to the 3 that I watched the most during my internship.
1. [Abhishek Thakur](https://www.youtube.com/c/AbhishekThakurAbhi/featured) - I found Abhishek's [*Implementing original U-Net from scratch using PyTorch*](https://www.youtube.com/watch?v=u1loyDCoGbE) video after completing 0toGANS. 
2. [Ken Jee](https://www.youtube.com/channel/UCiT9RITQ9PW6BhXK0y2jaeg) - Ken's videos taught me a lot about the business value that data can bring. He has videos on how he [*approaches learning through Kaggle*](https://www.youtube.com/watch?v=-pdXWmj9xxU&list=PL2zq7klxX5AQXzNSLtc_LEKFPh2mAvHIO&index=6) and many [*CV review videos*](https://www.youtube.com/watch?v=QBIe4nbmZfA&list=PL2zq7klxX5ARdms3L99sE8DTEsJ4_jCHP&index=24). Ken also started a #66daysofdata challenge where you can share your progress on any social media platform.
3. [Daniel Bourke](https://www.youtube.com/channel/UCr8O8l5cCX85Oem1d18EezQ) - Daniel brings so much excitement to data! My favourite series are [*Replicating Airbnb's Amenity Detection*](https://www.youtube.com/watch?v=C_lIenSJb3c&list=PL6vjgQ2-qJFeMrZ0sBjmnUBZNX9xaqKuM) and [*Machine Learning Monthly*](https://www.youtube.com/watch?v=DBbBRwpneLs&list=PL6vjgQ2-qJFdEjZjYFrwVZYlroGs5trip).

**TWITCH**. I didn't expect that I would use Twitch, especially when I was already comfortable (and probably a bit overloaded) with the content diet that I had curated. That being said, when you find a channel that produces quality content and easy-to-follow tutorials it's always good to make a note of them, so I can recommend → [*Cheuk's twitch stream*](https://www.twitch.tv/cheukting_ho). My favourites are the *Python Zero to Hero* and *The Legend of Data* series.

**MEETUPS**. These are great for keeping current and meeting people with similar interests to you. You might also get an opportunity to give a talk too. The meetups that I choose to join are typically Python or Data Science focussed, and have a mix of talks and tutorials. Some great places to find meetups and events are [meetup.com](https://www.meetup.com/) and [eventbrite.co.uk](https://www.eventbrite.co.uk/).


<img align="left" width="300" height="200" src="/images/tim-mossholder-unsplash.jpg">
 Needless to say, it is important to learn every day. When everyone was sent home at the start of the pandemic, I started the <b>#100daysofcode</b> <a href="https://twitter.com/_AnglinaB/status/1242181828120907784">twitter challenge</a>. This was super helpful for me as it provided me with accountability. Announcing what I was learning on social media forced me to structure my learning and pushed me to finish things that I started.  
 
Photo by [**Tim Mossholder on Unsplash**](https://unsplash.com/@timmossholder)

----------------------------------------------------------------------------

## What I'm up to now 👩🏽‍⚕️
Completing this internship has opened so many doors for me. I'm now working as a **Data Analyst** at [Railsbank](https://www.railsbank.com/) and will be starting a **Data Science MSc part-time** this September. I also started **collaborating on a project** with an awesome person who I met through [Twitter](https://twitter.com/aberasategi) (I'll save talking about this for another post). As my manager had mentioned a few times to **contribute to open-source projects**, I found through the [PyLadies Meetup Group](https://www.meetup.com/PyLadiesLondon/) the perfect opportunity to do this and have been able to contribute to [Pandas](https://pandas.pydata.org/docs/).

## Conclusion
I want to thank [GMV NSL](https://gmvnsl.com/) for having welcomed me. My internship was one of the steepest learning experiences that I've had the pleasure of encountering. Quite cheesy, but this journey has taught me that anything is possible. I went from minimal python experience to doing Machine Learning and software engineering, using geospatial data and point cloud data.

I hope this series of posts encourage you to find a learning path that best suits you, where some of the resources I recommended will be of use. Remember that there are so many resources out there and they all won't resonate with you, so don't be discouraged and keep trying. If you're able to, make a small amount of time to learn each day.

Thank you for reading.

