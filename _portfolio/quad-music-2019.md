---
title: "Music - 2019"
excerpt: "An updated analysis."
header:
  teaser: assets/images/lastfm-quadscrobbles.png
  
---

 

WHAT IS THE NARRATIVE


## Redoing 2018
I started by updating 2018 scripts 

### Top Songs

### Top Artists

#### R list

#### Chart
- updating to remove artists where song listens made up 75+% of listens

## 2019

### User Diffs 
- Song rank changes (Tableau)

### Artist Ranks

### Trendsetters


## Similarity

### Metric Thoughs

### Pair relationship matrix

### Things to learn

## Things Learned




------
alt structure
# Quad Music 2019

## Intro / Background
The release of [Spotify Wrapped 2019](https://www.spotify.com/us/wrapped/ "Spotify Wrapped") was the highlight of my first week of December. As my friends started sharing their Wrapped playlists in our group chat, I became increasingly eager to go home and get my hands on some new playlist data. 

2019 Wrapped was exciting because it was the first time I had more than one year of data for the same group of people -- giving me the opportunity to analyze how everyone's music tastes changed over time.

I also took it as an opportunity to improve my skills in data wrangling and data visualization using R and Tableau. 

## Group Analysis
- Top Songs
- Top Artists
	- R list
	- Chart (with update to non-user-dominated artists)
	- ranks

I plotted top 10 artists by number of song appearances (as either primary or featured artist) in 2018 and 2019. The initial version of the chart was dominated by artists who were heavily listened to by one person (some people *really* like their favorite artists), but I removed artists who had more than 75% of their song count coming from one listener. This was to get a better idea of what artists were liked by multiple group members.

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2019-topartists.png?raw=true "Top Artists 2018-19")

- Trendsetters
- **Similarity**

After looking at 

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2019-similarity.png?raw=true "Count of same artists between pairs of listeners")

This case probably requires some more advanced data ___ like clustering or network analysis.

At some point I will learn how to make a network graph, and things will get even more interesting. Once I figure out a way to get song genre information, it will be possible to link listeners together by similar songs and genres. This will be better than relying on the assumption that all artists stick to the same genre and that having one artist show up in two playlists means that the users have similar listening tastes.

	- metric thoughts
	- pair relationship matrix
	- clustering?

## Individual Analysis
- User diffs, song rank changes
- Tableau dashboard
