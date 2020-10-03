---
layout: default
title: "Particular Particles"
date: 2020-10-03 05:00:00 +0200
published: 2020-10-03 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,juice]
github: "https://github.com/zmalexander/"
noimage: true
---
# Particular Particles
Hello friends! Today we have a couple of visual updates, or 'Juice' as the industry likes to call it.
<!--more-->
A lot of the changes boil down to using a particle system, which is fortunately baked into Unity, but still required a bit of learning to figure out how to use it.

# Particle System
If we boiled down the Shoot your Friends experience to two main elements, we'd be left with Shoot and Friends. Both are impactful, so we wanted to make sure our fancy new particle emitters affected both.

When a player fires a bullet, it now emits a trail of particles. It's a somewhat subtle effect, but I thought it gave a little more 'oomph' to the shots. Likewise, when a player is killed they explode into a burst of particles. This is also adding 'oomph,' but to the act of murdering your friends.

In both cases, the particles are coloured to match whichever team the actor belongs to. I got to write a script for that which I'm pretty proud of.

# Other Changes
* The in-game scoreboard is made up of neon signs which will turn on to indicate who is in the lead (or tied for leader). The colour of the lighting corresponds to the team in the lead.
* Fixed a bug where the screen fade transition would end on an unplayable black screen.
