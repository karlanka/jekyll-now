---
layout: post
title: The impact of defending on scoring goals
---
## Intro
In this first post of mine I will try to show what impact defenders have on the chance of a goal being scored. If you read this you almost certainly know what expected goals are. If not [@11tegen11](https://twitter.com/11tegen11) explains it well [here](http://11tegen11.net/2015/08/14/a-close-look-at-my-new-expected-goals-model/). Rather than just performing some sort of correlation test and draw conclusions from that I build a bunch of expected goal-models based on logistic regression using different sets of predictors or features. 

Let's start with a case study:

https://github.com/karlanka/karlanka.github.io/blob/master/images/Paulinho%20defpressure%200.gif
https://github.com/karlanka/karlanka.github.io/blob/master/images/eddahri%20defpressure%204.gif

A fairly simple expected goal-model using angle towards goal and distance to the goal line assigns Paulinho's one-on-one with the goalkeeper an xG-value of 0.14. Eddahri's skillful, or lucky if you want, goal is said to have 17% chance of actually being a goal by the same model. A more sophisticated model incorporating further features such as assist type and if it's a direct shot or not would likely increase the xG of the first goal and decrease the value of the second to some extent. But any model that doesn't include defensive values would have a hard time correctly judge how good these two chances are. 

While I was almost done writing the code [@EightyFivePoints](https://twitter.com/EightyFivePoint) posted [something](http://eightyfivepoints.blogspot.co.uk/2017/09/bodies-on-line-quantifying-how.html) that was very similar to what I was doing. While this was a bit of a downer it at the same time it proved that my approach was not that stupid.

### Code
For those interested I have published the repo with the code for this post on my [github-profile](https://github.com/karlanka/). Most of the code live inside this [Notebook](https://github.com/karlanka).

### Data
[Stratagem Technologies](http://www.stratagem.co) have supplied data for this project. It includes all open play shots finished with either foot from the top tiers of Turkey, Switzerland, Sweden, Greece, Netherlands, Austria, Australia, Norway, Scotland as well as the second tiers of Germany and England.

This data includes, apart from coordinates, defensive pressure and number of defensive players between the finish and goal. A definition of the defensive pressure can be found in the notebook. Number of defensive players is rather self-explanatory - a one-on-one with the goalkeeper (or any other of the opposition's players) is putting this number at 1 (Paulinho's goal above). Eddahri's goal above have this numder at 2.

### Does a model with defensive features perform better than one without?
Without having any fur

### To what extent is the defensive features changing xG?

### Summary



**This article was written with the aid of StrataData, which is property of [Stratagem Technologies](http://www.stratagem.co). StrataData powers the [StrataBet](http://www.stratabet.com) Sports Trading Platform, in addition to [StrataBet Premium Recommendations](http://app.stratabet.com/recommendations).**
