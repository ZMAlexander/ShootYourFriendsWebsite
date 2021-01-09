---
layout: default
title: "The Final Mile"
date: 2021-01-09 05:00:00 +0200
published: 2021-01-09 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,juice,redesign]
github: "https://github.com/zmalexander/"
noimage: true
---
# The Final Mile
Hello friends! Well, it's finally almost happened. Shoot Your Friends is getting ready for launch.
<!--more-->
Much of the time spent between now and our last update was crossing Ts and dotting Is so that we could be ready to open up our Steam store page. We've only got a couple more hoops to jump through, and then we're officially ready for release!

That said, it's not like it's all been red tape here. Anybody familiar with software has probably heard about the Pareto Principle, that is that 20% of the cause achieves 80% of the effect. Or rather, that with a little initial work you can get a project most of the way there, but the final polish takes up to four times longer. We've been working on that final polish, and friends, I'm excited to tell you that I think this game is way sexier than it has any right to be.

## Steam Remote Play
Okay, so this is the coolest feature that we were able to implement. If you're not familiar with Steam Remote Play, the idea is that you can turn a locally multiplayer game into an online multiplayer game as long as somebody is hosting it. The best part for us is that it doesn't require a complete rework of the game's code - in most cases.

This was something that we were very excited to implement. Especially given the global health crisis, we were worried about releasing a game that was only available for multiplayer locally. Well, thanks to Steam, you can play this game just as well from two meters to two countries away.

So there's always a catch, right? Well, in most cases, this is just a plug-and-play setting that you set up, turn on, and away you go. But unfortunately that's not always the case. Without getting too bogged down in the technical details, we designed our player controllers a certain way, and I guess Steam expects them in another format. So the gist is that we got this feature working, but with some warts. There's a couple of bugs in here that we worked really hard to address, but they might be beyond us in a technical sense. 

Rest assured, we did confirm from multiple hosts that they're able to play the game. Before release, we're going to put together a tutorial demoing what that bug is exactly and how to get around it. We don't think it will greatly affect the player experience. But the flip side is that

## Background Crawl
Essentially from the start of development we've decided we wanted to have this outrun aesthetic, partly because we just missed the '80s and partly because it's this great mashup of lights and colours. So when we started, it was with a static background.

<img class="center-block img-responsive" src="/ShootYourFriendsWebsite/assets/images{{page.id}}/TitleBack.png" alt="Our original background image"/>

Well that's all well and good, but we can do better. At least, that's what Sara set out to do when she whipped up our new background. There was goint to be a city on the horizon, a city of excitement, possibility, and the shooting of friends. But that city was beyond the horizon, off in the distance, and nobody got anywhere staying where they started.

<img class="center-block img-responsive" src="/ShootYourFriendsWebsite/assets/images{{page.id}}/SyF_Background.gif" alt="A massively improved dynamic background"/>

So now we're zooming along the landscape, paying no heed to the darkness surrounding us. For we are heading for the city, for light, for possibility, and foremost: for deathmatch.

Migrating from a static image to a video did present a couple of technical challenges. There's a brief delay while the video loads into the scene. We're not super happy about it, but that might be a personal issue or something that we only notice because we're looking for it. If we start getting feedback concerning it, then naturally we'd want to address that.

## All the Colours of the Rainbow
Probably the greatest criticism we've given Shoot your Friends internally is that our levels feel somewhat flat. We've been working to address that, and came up with a solution that we think is pretty nifty.

We've set it up so that our levels can just *change colour*. These colours correspond to a team colour, which means that all players can be represented. 

To jazz things up a bit, we found two triggers to fire off this change. The first and most prevalent in our game modes, is to change the colour to whatever team is in the lead. The second behaviour is for our Juggernaut and Opportunism modes, where the player in control's colour will be reflected in the level. We figured both these behaviours indicate which players you want to watch out for.

## Counting Down to Awesomeness
Previously when playing the game, once all players were ready, they would choose their level, load in, and then were immediately thrown into gameplay. This felt a little bit jarring, so we wanted to introduce a little delay so that tanks weren't just suddenly flying around blasting each other.

Now when the game starts, the phrase "Shoot your Friends" will be narrated to the screen. It works pretty effectively as a three second countdown, which gives all players a chance to remember they're involved in a fight for their lives and to prepare themselves mentally to discharge their weapons into their friends.