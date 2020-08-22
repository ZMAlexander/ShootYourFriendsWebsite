---
layout: default
title: "gunsgunsguns And giveusatank"
date: 2020-07-18 05:00:00 +0200
published: 2020-07-18 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,bugs,UI,gameplay]
github: "https://github.com/zmalexander/"
noimage: true
---
# gunsgunsguns And giveusatank
Hello friends! For anybody out there still playing GTA3, the title of this update are cheatcodes that will show you a good time!<!--more-->
But if you are still playing GTA3, I'm sure you already knew that.

It's been a while since the last time we reached out, but that doesn't mean we haven't been busy! In fact, we've been so busy we sort of lost sight of this whole outreach / blog thing which I recognize as a failure on our part. We'll try to do better in the future.

But you're probably not here to hear us whine about our schedule, or even for twenty-year-old cheat codes, so let's get into the update details:

# GunsGunsGuns
Shooting your friends is great and all, but having just one gun to shoot with? Nah, forget that. We've added four new guns to the game, with plenty more on the way! Now you can shoot your friends in whatever manner you choose!

## Spread Gun
The Spread Gun is a classic weapon in any shmup. I want to say it dates back to Contra, but I'm sure it's even older than that. Our take on the Spread Gun is a weapon that fires five projectiles in a tight fan around the player.

The standard gun only fires one projectile in a straight line, so you wouldn't be mistaken to think that the Spread Gun is much deadlier (five times deadlier, in fact). While we're not anticipating a high stakes competitive scene for SyF, we are keeping an eye on balancing various weapons. To this end, you'll notice that the Spread Gun has a relatively short range.

## Burst Gun
This is a gun that brings more dakka to the table. The Burst Gun fires three projectiles in rapid succession straight ahead of the player. This makes it pretty well impossible to dodge parallel to the bullets, so watch out!

We're still trying to find the sweet spot for balancing this weapon. Right now we're experimenting with range, projectile speed, and fire rate. Overall, the weapon feels nice in its current state, but I'm not sure if it's reached perfection yet.

## Ricochet
It's hard not to appreciate a certain element of chaos in a party shooter, and the Ricochet brings exactly that. The Ricochet fires a standard bullet which bounces off of other surfaces - including other bullets! That'll keep everyone on their toe.

## Magnum
The Colt .44 Magnum is the most powerful handgun around. Unfortunately, we don't own the rights to Colt or Dirty Harry, so you'll have to make do with our version of the Magnum.

Firing the Magnum causes knockback to yourself and the screen to shake. Overall, I'd say it's the gun with the highest fun factor in our collection.

We did have a discussion about really going ham with the Magnum and adding some screen flash to firing it. In the end, we discovered that we don't really like that sort of thing in the games we already play, so we've decided to leave that one out. Our eyeballs thank us for that.

# GiveUsATank
Since day one we've wanted to put multiple playable characters into our game. We've had a stick figure for debugging and have basically left at that while Sara whips up some characters we're all happy with. We've come to the point however where we needed to start programming character selection.

I've whipped up a sample of what a tank might look like as a player. This demonstrates two things for us:
1. It's now possible for the player to select from multiple characters available to them
1. I should not be allowed to draw or design characters for our game

The tank is incredibly rough, and will probably only be available to us in the development builds for testing. Still, being able to choose a character is an incredibly significant feature worth sharing with you.

# Bug Fixes
It wouldn't be our game if we weren't introducing bugs. That said, we must be getting better about introducing bugs with our changes, as there aren't a whole lot with this update:
* Fixed an issue where a player would spawn clones of itself if it was struck by a bullet more than once in a frame. This was an exceedingly rare occurence until we introduced the spread gun, where suddenly every player killed spawned a bunch of clones. (This was actually hilarious, and is inspiring a game mode down the line for us)
* Fixed an issue where after the players have already played a game, they will enter the next level and be unable to kill each other. Doomed to forever wander the purgatory that is the SyF arena, unable to feel the sweet release of death.
* Fixed an issue where the in-game pause menu filled the entire screen
