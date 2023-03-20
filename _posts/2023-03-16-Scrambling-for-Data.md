---
layout: post
title:  "Scrambling for Data"
author: Brannon Olive
description: Finding and creating useable data from professional golfers.
image: /assets/images/golfBall.jpeg
---

## Background

The data that I found was different stats from professional golfers from this year. To figure out whether or not this data was ethical to scrap from ESPN,
I looked at the robot.txt page. I found the urls of the pages that I wanted to take the data from and looked if the extensions were on the disallowed list.
I did not find any of the extensions on the page so I decided that there wouldn't be anything wrong with using this data.

Here are links to the two pages where I got the tables from:

[Golfer Stats](https://www.espn.com/golf/stats/player)

[Golfer Ranks](https://www.espn.com/golf/rankings)

The data was not all in one table, so I did have to take each table off one by one and join them together. On ESPN, I found a page that had most of these stats for each player. 
The big one that was missing was the ranking. So I scrapped the web page for the table with the stats and did the same for the table with the rankings. Before joining, I had to make 
sure to drop the ranking from the table with the stats on it because I wanted the final ranking to be the overall ranking and not their ranking for that specific stat. 
Once that was dropped, I just merged the two tables together using their names as the key to join on. The one problem with my data is that there is a lot of golfers who 
are no longer on the PGA Tour but are still on the world rankings. The stats for players not on the PGA Tour is not as available as for the golfers who do play on the Tour.
Here is an example of the data and a few of the top ranked golfers.


![Figure](https://raw.githubusercontent.com/bolive2/my386blog/main/assets/images/GolferChart.png)

## Goal

The data includes several stats that are important parts of golf as well as the ranking for golfers that have prefromed good enough to receive one. I want to look 
at the data and see which stats are common among the top golfers and which ones lead to a golfer not being ranked as high. These stats inlcude things like how far 
on average a golfer drives the ball and how many putts it takes them on an average hole. There is a lot that goes into being a top ranked golfer and even the best golfers 
in the world have strengths and weaknesses to their game. I want to see which strenghts are the best to have and which weaknesses hurt the most.

By my next blog post, I want to be able to see what things golfers should work on the most to improve their game. I am hoping that by seeing the trends among the professional
golfers, I will be able to see what ways the top golfers are able to seperate themselves from the rest of the pack. 

Here is a link to the github repository with the code I used: [Github Repo](https://github.com/bolive2/golfData)
