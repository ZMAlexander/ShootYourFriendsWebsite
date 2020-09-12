---
layout: default
title: "Polishing Guns"
date: 2020-09-12 05:00:00 +0200
published: 2020-09-12 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,guns,juice]
github: "https://github.com/zmalexander/"
noimage: true
---
# Polishing Guns
Hello friends! This week our focus has been on making improvements to the look and feel of our weapons. If you're going to be shooting your friends, it better make you feel something after all !
<!--more-->
This week I'm sure also marks the beginning of a trend where we're going to be going around adding polish and juice to Shoot your Friends, so I imagine you'll be seeing a lot of updates similar to these in the near future.

# Bugs
The burst gun, a weapon which fires a three-round-burst in a single direction, was having just the strangest issue where the player was not able to shoot downwards with it. After poking and prodding, we discovered that the bullets were colliding with the player when firing downwards, but not in any other direction. We've gone ahead and fixed it so that bullets don't collide with the player who fired them, so that's just not an issue anymore.

# Polish
Up until this point, all of our weapons had the same sound effect. That worked fine when you switched from the standard gun to the burst gun, ricochet, or perhaps even the spread gun. But it certainly sounded weird for the rocket launcher and flamethrower. We've gone ahead and made sure weapons that should sound unique do - in fact - sound unique. 

Speaking of sound effects, we've really played up our rocket launcher and are super proud of it. The rocket's operation is now a sum total of three different sound effects: a 'fwump' when fired, a 'ssss' when airborne, and a 'ka-pow' when it explodes. Overall, this was a super simple thing to implement, but my goodness does it ever feel more right to use the rocket launcher now.

Appropriate weapons now also generate little muzzle flashes when fired. This isn't an earthshattering change, but it was fun to implement. However, things look a little funky right now since our stand-in players don't have any guns! But at least we've proven the concept.



