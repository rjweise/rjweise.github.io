---
title: Article - Are NHL referees biased towards certain teams or home teams vs. away
  teams?
date: 2018-02-02 00:00:00 Z
layout: post
---

### A research project using NHL API Live Feed json files from the 2010-2011 season until Jan. (incl.) of the 2017-2018 season.

I ran into [an interesting website](http://scoutingtherefs.com) by Joshua Smith, and after reading some of the content and playing with the data I decided to look for some more detail. Using R ([code](https://github.com/rjweise/RESEARCH---NHL-Referees/blob/master/Rcode-NHLGameJSONperSeason)) I downloaded the basic information I needed to analyze and visualize in Tableau Public.

### Data

After downloading all Game Summary files wit specific columns needed for my analysis I combined the files per season and cleaned them up in Excel (removing all repeating headers and a weird record at the end of the file). From there I loaded them in Google Cloud Storage, and used Google Big Query to union all files in to one (only Penalty events).

### Tableau

Things to look at:
* penalties per period / game
* penalties given to home or away team
* penalties given per referee(-combo) per team (favoritism?)
* when are the penalties called during the game?
* at what score are penalties called?
* penalty call locations
* penalties over season since 2010, per penalty type
* etc.

-to be continued-
