---
layout: default
title: "Facelifts and Rockets"
date: 2020-08-29 05:00:00 +0200
published: 2020-08-29 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,guns,ui]
github: "https://github.com/zmalexander/"
noimage: true
---
# Facelifts and Rockets
Hello friends! Today, like usual, we have a bit of a hodge-podge of new features.<!--more-->
But before we get into that, I wanted to recognise that we haven't been great about keeping up with our weekly updates. Sometimes we lose sight of that, but all we can do is try to do better in the future. So if this update doesn't look like there's a lot going on, it's probably because we've been in the habit of giving you a few weeks' worth of updates all at once!

Actually, while we're on the topic of minor updates, some of our developers are in the process of buying their first houses. If you've been a first-time homeowner before, you probably remember it being a blend of excitement, stress, and generally pretending to be an adult. At least, I hope you do, that's been my experience. Anyhow, that's eating a lot of our time in addition to our day jobs. We're expecting development to slow for a while without stopping entirely.

## Rocket Launcher
In our last update we added a plethora of new guns to play with. But one notable member was missing from the cast of deathmatch weapons, and that's the Rocket Launcher. A projectile is fired and detonates when it collides with an object or person. Any enemy caught in the blast is killed, which makes this the ideal weapon when your opponent is sticking to cover or if your aim isn't so hot.

Offensively, the Rocket Launcher seems like a great weapon. But we've got a few tactics to face off against it. The Rocket Launcher's preferred terrain is one strewn with obstacles, so it's a pretty poor weapon if you're fighting out in the open. The rocket is also on the slower end of most of our projectiles, so it's susceptible to being dodged. Finally, the rate of fire is our slowest yet, so you really need to make your shots count or else you'll be in trouble.

All in all, we think this is a natural inclusion to Shoot your Friends. It's a legendary weapon in the genre, but not one without its warts.

## User Interface
We've been going around cleaning up our menus so they're more usable. Our two major changes here are on the Player Lobby and the Level Select screens.

In the Player Lobby we've done pretty much a total overhaul. Since the inclusion of customizable weapons and skins, we've been sort of tacking on new menus for the player to scroll through. One thing that we were lacking was some consitency between all of them, so we've blended them together into something we're satisfied with. We're not sure this is what the final Lobby will look like at release, but it's definitely a lot cleaner than our original wireframe.

Moving on to the Level Select screen, we've also applied some consistency updates. Now each scrollable field - such as game modes and the levels themselves - follows the same design as in the rest of our game. This appears cleaner and more consistent. We've also added in a loop to the level selection itself. We thought this would make it easier to scroll endlessly through the available levels, or return to the start of the list.

