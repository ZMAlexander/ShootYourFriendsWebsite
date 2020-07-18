---
layout: default
title: "Announcing Fancy Pigeon Studios"
date: 2020-07-18 05:00:00 +0200
published: 2020-07-18 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,bugs,UI,gameplay]
github: "https://github.com/zmalexander/"
noimage: true
---
# Announcing Fancy Pigeon Studios
Hello, friends! It's been a while since our last update, and we've been cooking up something very special in the meantime. 
<!--more-->
Us folks working on Shoot Your Friends are nearing a release candidate, which means we've been getting our ducks in a row to start submitting the game to various stores. One of the common requirements amongst platforms is that we need to be operating as an official business, so we've been speaking with lawyers and accountants and such. The end result is that we're now incorporated as Fancy Pigeon Studios Ltd.

On a personal note, this is a huge milestone for me. I've always wanted to run a studio in the video game industry, and now I have the paperwork to prove I've advanced from hobbyist to professional. I really couldn't be happier!

# Okay, but what about the game?
While this whole incorporation process has taken a lot of our time and energy, we'd be pretty remiss if we didn't keep putting effort into developing our product! Rest assured we have a few new things to look forward to:

## New Game Mode
We've created a new way of playing the game, which we've tentatively titled Opportunism. Essentially, only one team is allowed to score points at a time. The team that is allowed to score will be randomly selected every few seconds. This introduces a high degree of chance to the game, which we recognize is a divisive issue between different types of players.

To the best of our knowledge, this is a unique game mode. I mean, surely somebody's done it before, but I can't think of what game that might have been. As such, this is a really kind of experimental mode and we can expect to be making more refinements before release. For instance, I'm not super happy with the name "Opportunism" - if you have a better one please let us know!

## User Experience
Software lives and dies by the user experience, and I believe video games are no exception. We've been hard at work making sure the game feels good to play - from the menus to the gameplay itself. Here's a couple things we've worked on:

* We've added a loading screen to not only prepare the level for better performance, but it also gives the players a chance to confirm their readiness and read the controls.
* The volume options has had an additional slider added to it separating the music from the general sound effects. We recognize that you've got your own tunes to play to, and that's totally cool with us. We've also taken this opportunity to clean up a few sound effects which weren't affected by the volume slider.
* We've greatly expanded the score limits for various game modes, and made them make some more sense. For instance, Deathmatch can go up to 25 points instead of the original limit of 9, and the player no longer needs to scroll all the way from 1-25 individually to get there. We've also renamed the score limits to be more descriptive of what they are - eg "Kills" for Deathmatch modes, "Minutes" for timed modes, etc.

## Bug Fixes
> *99 bugs in the program's code,*
> *99 bugs in the code,*
> *Take one down and patch it around,*
> *108 more bugs in the code*

Sometimes things don't take a linear path when you're working on them. For instance, we had an issue where under certain circumstances the player could shoot straight through a wall. That's a pretty major issue, so we fixed that straight away - only it introduced a new issue. Now bullets could pierce into a wall and get stuck inside them. That's less dangerous but visually unappealing so we resolved that too. This fix introduced another issue where bullets would just randomly be destroyed even if they didn't collide with an obstacle. That was major so we fixed that too. Now the bullets appear to be working just fine - except that they can still sometimes strike a player through a wall while the bullet is being cleaned up. We're still working on that one.

Fortunately, we've also got a bunch of bugs that we put to bed for good:

* Levels were not entirely visible on display ratios that did not match 16:9.
* When choosing a level it was possible to keep scrolling past available levels and into the aether.
* The player could sometimes dodge into a wall and become stuck.
* The countdown timer for Timed Deathmatch would appear off screen somewhat
* Issues with Timed Deathmatch prevented a Draw from being declared. This would sometimes cause the game to not end until the tie was broken, and in other circumstances would randomly declare a winning team instead.
