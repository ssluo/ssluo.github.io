---
title: "Music - 2019"
excerpt: "An updated analysis."
header:
  teaser: assets/images/spotify2019-preview.png
  
---

The release of [Spotify Wrapped 2019](https://www.spotify.com/us/wrapped/ "Spotify Wrapped") was the highlight of my first week of December. As my friends started sharing their Wrapped playlists in our group chat, I became increasingly eager to go home and get my hands on some new playlist data. 

2019 Wrapped was exciting because it was the first time I had more than one year of data for the same group of people. Not only could I repeat and revamp [last year's analysis](https://ssluo.github.io/portfolio/quad-music-2018/ "Music - 2018"), this year opened up the possibility of analyzing how music tastes changed over time. 

This was also a great opportunity to improve my skills in data wrangling and data visualization using R and Tableau.

## Group Analysis

**Top Songs**  
Same as last year, I found all the songs that appeared on multiple playlists and compiled them into one playlist for the group to use at will. This year was heavily dominated by Billie Eilish, Ariana Grande, and Allie X, which leads us to the next part...

**Top Artists**  
*[in progress: R list, ranks]*

I plotted top 10 artists by number of song appearances (as either primary or featured artist) in 2018 and 2019. The initial version of the chart was dominated by artists who were heavily listened to by one person (some people *really* like their favorite artists), but I removed artists who had more than 75% of their song count coming from one listener. This was to get a better idea of what artists were liked by multiple group members.

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2019-topartists.png?raw=true "Top Artists 2018-19")

**Trendsetters**  
*[in progress]*

**Similarity**
To get a simple idea of which friends' listening tastes are more/less similar to others, I counted the number of shared music artists for each possible combination of listeners. However, this method 

I am currently creating a metric that incorporates song similarity, adjusting the similarity score up if a pair of users have the same song appear on their playlists.

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2019-similarity.png?raw=true "Count of same artists between pairs of listeners")

My next goal is to find song genre data: that will make it possible to link listeners together by similar songs *and* genres. This will be better than relying on the assumption that all artists stick to the same genre and that having one artist show up in two playlists means that the users have similar listening tastes.

Also, this case probably requires some more advanced analysis methods like clustering or network analysis (to evaluate groups of people, not just pairs).

## Individual Analysis
I also created summaries of how each person's listening changed. Some friends had over 50% of their Wrapped playlist stay the same from 2018 to 2019, while others had only 7 songs remain the same. 

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2019-samesongs.png?raw=true "Count of same songs in both playlists, by user")

For each user, I plotted the yearly ranks of each song that appeared in both years. 

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2019-indivdash.png?raw=true "Serena's dashboard")

Future plans for this dashboard include: a) creating a genre composition for each year's listening and comparing across years and b) adding total listening stats (from Last.fm).