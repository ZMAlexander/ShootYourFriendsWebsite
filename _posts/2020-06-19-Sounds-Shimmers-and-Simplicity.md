---
layout: default
title: "Sounds, Shimmers, and Simplicity"
date: 2020-06-19 05:00:00 +0200
published: 2020-06-19 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,juice, music,UI]
github: "https://github.com/zmalexander/"
noimage: true
---

# Sounds, Shimmers, and Simplicity
Hello friends! This week we've been making some continuous improvements to the game - which is what we do every week. 
<!--more-->

## Sounds
This is going to be hard to write about without simply being able to show it to you, but we've added the ability to play music in our game. We haven't landed on a final track list yet, but it's good to have something to rock out to while you're shooting your friends.

Additionally, we've added a number of sound effects to the game. Our menus have a more complete look and feel, and will now "chirp" as you select different buttons. We've also played with our bullet sound effects and fixed an issue where your gun would suddenly cease making noise when a bullet struck an object. It could be jarring.

## Shimmers
We added a new game mode which we're currently calling Juggernaut. The rules of Juggernaut are carried over from a few different games, but they might not be readily apparent. Juggernaut is a deathmatch ruleset where one player (or in our case a team) is considered to be the Juggernaut. When the Juggernaut kills a player they gain a point, but when a regular player kills a player they don't. If a player wants to become the Juggernaut - and let's face it, they do - they must first kill a Juggernaut and gain their power. It's a gamemode that rewards streaks of kills, and punishes simply trading them back and forth.

One of the requirements to have a mode of play like this is that it must be immediately apparent to the players who the Juggernaut is. We achieved this effect by showing the affected player to be crackling with electricity. It also makes a pretty nifty trail behind the player as they run.

<img class="center-block img-responsive" src="/assets/images{{page.id}}/juggernaut.gif" alt="Our special juggernaut animation in action"/>

There's a couple of issues with this implementation, but we're happy with it for now. Something that is on our radar is that there are some optimization concerns with this effect. I consider my development machine to be a pretty beefy gaming rig, but it ran into some stuttering when calculating lightning bolts. We played with it until that frame loss disappeared, but we recognize that this might be an issue on different hardware.

## Simplicity
Part of the feedback we got from our testers was that some of our UI elements were difficult to use with a gamepad. That's especially concerning to us, given that our game is intended to be used solely with a gamepad.

We've taken a hard look at our pain points and addressed a number of them. For instance, there were some dropdown menus on our options screen for controlling video quality. This is a perfect implentation for a keyboard user, but rather difficult to use with a controller. We've instead replaced it with a list you can scroll through by pressing the left or right buttons.

Speaking of scrollable lists, we also recognized and opportunity to use them on our level select screen. When choosing a gamemode or score limit, we would previously require the player to move to the left or right button, and then confirm that selection. We've cut out the middle man, and it makes for a much smoother experience.