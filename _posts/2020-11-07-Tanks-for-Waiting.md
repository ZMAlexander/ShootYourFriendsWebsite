---
layout: default
title: "Tanks for Waiting"
date: 2020-11-07 05:00:00 +0200
published: 2020-11-07 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,juice,redesign,player]
github: "https://github.com/zmalexander/"
noimage: true
---
# Tanks for Waiting
Hello friends! Today we're announcing a return to work along with a bunch of other changes.
<!--more-->
You might be wondering "*Why the delay?*" and that's a fair question. Fancy Pigeon has been in the middle of changing its address for a while now, which sort of stalled out work. Requiring a lot of energy is something that moving and game design have in common, apparently. However, in the week we've been back we've made a ton of changes, so I think you might be pleasantly surprised.

## A New Challenger Approaches
Our principal art director really outdid herself this week with our new player model: a retro-futuristic tank. We're all very impressed with it, and it does indeed make Shoot your Friends look like a professional endeavour.

<img class="center-block img-responsive" src="/blog/assets/images{{page.id}}/player.png" alt="The new player model"/>

We were excited to put the tank in play, and perhaps a little too eager. When we entered this project, the original design was going to be human characters, with facings in one of two directions and being able to shoot at compass points. That didn't really translate well to this tank model, so some significant changes were made. The player now shoots in the direction they're facing, which means we now support shooting in any direction as the player rotates.

<img class="center-block img-responsive" src="/blog/assets/images{{page.id}}/twist-and-shout.gif" alt="Our new player model moving and shooting in 360 degrees"/>

That was a significant enough overhaul, but we didn't stop there. All of our audio direction was based on humans as well. We've replaced the footsteps with engine noises and the laughter for taunting is now a horn (Ford Model A - very exciting!). Plus, just because we thought it was neat, the players now leave a coloured trail behind their vehicle as they move.

## Other Changes
* Fixed an issue where the dodge cooldown display would rotate with the player
* Fixed an issue where the game would freeze when changing between scenes
* The victory banner's text is now coloured to match the winning team