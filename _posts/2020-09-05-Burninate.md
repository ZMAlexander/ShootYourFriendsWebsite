---
layout: default
title: "Burninate"
date: 2020-09-05 05:00:00 +0200
published: 2020-09-05 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,guns,modes]
github: "https://github.com/zmalexander/"
noimage: true
---
# Burninate
Hello friends! This week we've added a new weapon to play with, and from the title of this post I bet you can guess what it might be.<!--more-->
Not only that, we have a new gamemode to introduce, and a couple of juicy additions we've been working on too!

# Flamethrower
That's right, by playing Shoot your Friends you're now preparing yourself to commit warcrimes by using the flamethrower! Mechanically this weapon has an insanely high rate of fire, which means you never need to stop shooting. But before you start roasting marshmallows on your buddies, there are some significant tradeoffs. The range of the flamethrower is quite short, and you are slowed while using it. Additionally, flames don't intercept bullets like other bullets do, so the flamethrower's defensive potential is quite limited. Still, it's a flashy weapon for flashy people, so get out there and get fired up!

# Sponge Mode
We've also added a new game mode which we're calling Sponge. The name comes from the term Bullet Sponge, which for the uninitiated refers to something in a video game you must shoot but has tonnes of health. In this gamemode, players have a pool of health instead of a number of lives, and play proceeds until all but one team is elminated. In essence, it's a lot like Stock mode but without respawning.

Introducing Sponge at the same time as the flamethrower had an interesting interaction though: if a player hit an opponent with a flamethrower they would basically win the game immediately. The flamethrower's rate of fire is just so high (it fires 20 times per second). To rectify this, we've added an invulnerability effect to the game. Now when a player is shot, they are invulnerable for a couple of seconds. Of course, in most games getting shot simply kills the player, so it's something you'll only really see in Sponge.

# What Happens When I Get Perforated
We've made a couple of changes this week as well, and they both have to do with getting shot. When a player is killed, they now play a sound effect. It gives a little bit more impact to the act of homicide, and we're exploring more ways to jazz that up.

Additionally, it was too easy for a player to accidentally get killed at spawn. Since we just introduced an invulnerability timer for Sponge Mode, we decided it made sense for a player to spawn into the game with a brief period of invulnerability. That way they at least have a chance if someone's suppressing the spawn points.



