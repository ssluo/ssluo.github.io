---
title: "Music - 2018"
excerpt: "Analyzing music listening trends among my friends."
header:
  teaser: assets/images/lastfm-quadscrobbles.png
---

My friend group, self-titled "the quad", likes to share what music we're listening to with each other. What started out as a collaborative playlist on Spotify has turned into competing for weekly highest song listening counts and playing games to see how well we know each other's music tastes. 

With an abundance of data from Spotify and last.fm, I took the opportunity to make some charts.

## Weekly Listening Stats
One friend created an app called [this-week-fm](https://this-week-fm.herokuapp.com/home "this-week-fm") to track the last.fm listening stats of everyone you follow. By following every other friend's last.fm profiles, we could keep up with what music they were listening to and casually compete to listen to more songs per week. 

I used the app to record a few weeks of listening statistics for the group, and used R to chart trends.

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/lastfm-scrobblesperweek.png?raw=true "Quad individual weekly scrobble counts")

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/lastfm-quadscrobbles.png?raw=true "Quad total weekly scrobbles")

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/lastfm-weeklyranks.png?raw=true "Weekly individual rankings")


## Spotify Top Songs 2018

I used the Rspotify package and the Spotify API to collect each friend's Spotify-made playlist of their top 100 songs in 2018. Using this data, I was able to find out what artists were most heavily listened to in the group.

![alt text](https://github.com/ssluo/ssluo.github.io/blob/master/assets/images/spotify2018-topartists.png?raw=true "Quad top artists 2018")

I also used the combined playlist data to make a Spotify playlist in which every song is enjoyed by at least two people in the group, and tested it at a gathering. Feedback: enjoyed!