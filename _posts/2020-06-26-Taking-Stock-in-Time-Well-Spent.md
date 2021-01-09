---
layout: default
title: "Taking Stock in Time Well Spent"
date: 2020-06-26 05:00:00 +0200
published: 2020-06-26 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,bugs,UI,gameplay]
github: "https://github.com/zmalexander/"
noimage: true
---

# Taking Stock in Time Well Spent
Hello friends! This week two new game modes have been added to Shoot Your Friends, so let's dig in
<!--more-->
and see what they're all about!

## New Game Modes
Before we get in to what these game modes are, I just wanted to take a minute to gush. Early in our development cycle, we recognized that the thing we'd like to separate Shoot Your Friends from the crowd would be the number of ways to play the game. We started with a simple concept (a concept that can be boiled down into the title of the game), and were delighted with how many ways we could twist that. 

So with that in mind, we spent a considerable amount of time early on in planning our Rules engine. Now, for those not familiar, a Rules engine defines how the game plays, what the conditions for victory are, etc. It's not a strictly necessary component, but it's an important one to us. Without something like this engine, adding a new game mode could quickly spiral out of control and take weeks or even months of development time. Ours typically take a day or two.

It's not a perfect system yet - the quick returns on new game modes seem to introduce new bugs that we hadn't considered - but I'm super proud of it. So without further ado, let's talk about these new modes.

### Stock 
I think this mode is pretty intuitive, and anybody who follows the Smash Bros franchise probably already knows how it works, but Stock is a twist on Last Team Standing. Each team gets a pool of lives, and whenever they're killed they use a life to respawn. Eventually, friends will shoot each other enough that those lives will run out and the game becomes a battle for survival.

The shared life pool was an important decision to us for a couple of reasons. On one hand, it can keep teammates covering each other - that way Player 1 doesn't have to pay for Player 2's mistakes. On another hand, the shared life pool can also be used to punish a team - it's a potent handicap against teams that are made of players of disparate skill levels.

A third consideration for us was that it was the easiest method to implement. I want to be clear that wasn't the reason we ultimately decided on it, and there wouldn't be anything stopping us from adding in an individual life pool mode, but sometimes you just get lucky like that.

### Timed Deathmatch
This is basically exactly what it says on the tin. Timed Deathmatch follows the regular rules for Deathmatch, being that each time you shoot someone on the opposing team you score a point. The twist here being that instead of playing until you reach a score limit, you're playing until time runs out.

Adding this twist in made this the most architecturally challenging mode to date. None of our other game modes care about the passage of time, so we had to figure out how to set up a clock and keep it communicating between different components. Unity does most of the heavy lifting for us in order to keep track of time between frames, but we were surprised that there wasn't an out-of-the-box solution for making a timer or clock.

<img class="center-block img-responsive" src="/assets/images{{page.id}}/timer.png" alt="This may be the simplest clock in video games"/>

In the end, we figured it out. It turned out making the clock and keeping time is a relatively simple problem. Or at least it is with the level of help our engine gives us.

Another fun thing about putting in a clock: this is the first game mode that it's possible to score a draw in. We don't actually have a system in place for that yet - player number is the determining factor in tie games. That's not something we're super happy about, so you can be sure we'll be figuring out how to make tied games soon.

## Other Stuff
It's not the intention of this blog to be simply posting patch notes in here, so I'm just going to give the highlight reel of stuff we fixed this week:

A long-standing issue where players would get stuck against walls has been smoothed out. Movement feels really nice now, and players can slide along walls or squeeze through gaps without needing to worry about getting hung up on something.

A number of our game modes were having issues if you set the score limit to 1. We figured out what was causing it and fixed it, so now you can have really short games if that's what your heart desires. 

Speaking of game mode settings, we've added a neat quality of life feature where if you go in for a rematch or to play a new level, your settings are saved. No longer do you have to flip through the list to get things just right every time (It's worth noting that going to the lobby overrides this feature. We figured you'd go there to add a new player into the game, and that probably changes the type of game you want to play anyway).

Fixed a number of issues related to sound effects. In some scenes, certain effects would collide with each other. Our primary example was when everyone is ready on the lobby screen, a special effect is played. At that same time, in the next scene a UI element is selected and chirps. The two sound effects were overlapping with each other, so we squelched the UI effect. It sounds much nicer as a result.

Speaking of sound effects, we found a number of sounds weren't affected by the volume slider in the options screen. We've since fixed a number of sounds.

