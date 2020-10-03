---
layout: default
title: "Improving Quality of Life"
date: 2020-07-18 05:00:00 +0200
published: 2020-07-18 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,bugs,UI,gameplay]
github: "https://github.com/zmalexander/"
noimage: true
---
# Improving Quality of Life
Hello, friends! Since our last update, we've been working hard at swatting bugs and improving quality of life. 
<!--more-->

## Gameplay Bugs
* Stock mode allowed players to go into negative lives
* Stock mode ended when players ran out of reserve lives, and not when all players on the team were killed
* Under certain condition, a player could be killed if touching a wall that a bullet struck the opposite side of

## Level Selection Bugs
One of the thorns we've encountered has been our level selection screen. Early on, we had decided we'd like to have navigation resemble a carousel, but we weren't sure how to implement it. Eventually we muddled through it, but we uncovered - or perhaps introduced - a number of bugs in the process. 
The level selection screen has received a great deal of love, so many of our resolved bugs are related to that:
* On the level selection screen, the navigation buttons could become unreachable by gamepads
* Selecting a level could sometimes change the game mode
* Certain levels were unreachable via gamepad
* It was possible to scroll past the total available levels on the level selection screen

## Quality of Life Improvements
### Settings
One of the things that should be a no-brainer yet somehow wasn't included in our game was the ability to save your audio and video settings. Talk about an oversight! Whether that's a feature or a basic requirement, we've gone ahead and added the ability to do that. We also noticed some issues where the Options menu would show the default settings instead of what the active settings are, so we went ahead and fixed that too.

### Game Modes
Almost all of our experience with our testers indicated that there was some confusion about how to play certain game modes. In a bid to rectify this, we've added an information dialog for each game mode. This is a window that can be brought up explaining what exactly the game mode is. Hopefully that clears things up!

### Loading Times
Nobody likes waiting around on loading screens, so we've optimized our algorithm to get you back to shooting your friends faster.