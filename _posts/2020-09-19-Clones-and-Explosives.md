---
layout: default
title: "Clones and Explosives"
date: 2020-09-19 05:00:00 +0200
published: 2020-09-19 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,guns,gamemode,juice]
github: "https://github.com/zmalexander/"
noimage: true
---
# Clones and Explosives
Hello friends! It's been a pretty busy week here at Fancy Pigeon, with a new weapon, new gamemode, and what feels like a bazillion tweaks and bug fixes.
<!--more-->
Let's jump right into it

## Simulacra Mode
This game mode plays just like the Stock mode rules. That is, players will fight it out until their team runs out of the lives. The big difference here is that all of your lives are spawned at once, so each player is controlling multiple characters. This feels odd, and maybe even a little whacky, but we thought it would make an interesting addition.

Fun Fact: This mode was inspired by a bug we were experiencing with the spread gun. It turns out that the nature of that weapon may cause multiple projectiles to strike a player at once, and each projectile was a trigger to spawn a new player. We've fixed that bug, but added this mode because, frankly, we thought it was a hilarious interaction.

## Grenades
It seemed a shame to use our ultra-cool explosion effect only on the rocket launcher, so we decided to give the player access to grenades as their primary weapon. A projectile is thrown a short distance away, and detonates after a brief delay. If we're comparing it to the rocket launcher, the range is much lower, but the rate of fire is much higher. We've found that it makes an excellent defensive weapon, as you can throw grenades behind you while on the run.

The grenade also represents our most complex animation to date, which in fairness is not saying much. We wanted the grenade to appear to spin in the air, as well as appearing to travel in an arc. We had some trouble conceptualizing what an arc might look like in a top-down game. In the end, we achieved our desired effect with a simple growth/shrinking animation. We're pretty pleased with it!

## Polish
As is becoming the norm at this point in development, most of our work is on polishing the game. Here's an itemized list of what we did:

### Features
* After completing a round, the player is presented with an option to play a rematch. A rematch will be on the same map with the same players and weapons.
* Some 'safe spawning' logic has been added to the player spawner. The need for this became most apparent in Simulacra mode, where some of the players' clones would spawn adjacent to their opponents.
* The player may now press a button to play a taunt voiceline at their opponents.
* Scene transition effects have been added.
* At the end of the round, instead of displaying the points total with the generic descriptor "Score," we will now be using a more relevant descriptor based on the game mode. For example, Deathmatch now reads "Kills," and Stock mode reads "Lives"

### Bugs
* The character preview window on the lobby appeared to be squashed for some skins.
* Fixed overflowing text on weapon selection menu.
* Players are no longer able to start a game before any player sets themselves to 'ready.'
* Explosions were deadlier for far longer than they should have been. A player is now safely able to walk into the smoke left behind from an explosion.
* Being struck by the spread gun was causing players to spawn multiple instances of themselves.
* Resolved an issue where the player would flicker between two different skins.
* Resolved an issue where the Ricochet gun would bounce off explosions and flames as if they were a solid wall.



