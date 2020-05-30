---
layout: default
title: "Welcome to Shoot Your Friends blog"
date: 2020-05-11 05:00:00 +0200
published: 2020-05-11 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends]
github: "https://github.com/zmalexander/"
noimage: true
---

## Pregame Lobby
Arguably, one of the first things a player will do when they start the game is try to start the game. 
<!--more-->
We think this is a fair and justified response, and take our players to the pregame lobby. This is a screen that's probably familiar to you, where each player pushes a button on their gamepad to enter the game.

![The pregame lobby in action](lobby5.gif)

This screen has a surprising amount of complexity to it. Each player is going to use a different gamepad. They might decide to back out after they've started so they can change their avatar's skin. Controllers might get swapped out when your host gives you a knock-off controller. Fortunately, our engine (Unity - for anybody curious) has a new component that helps us keep track of which players belong to which controllers. Unfortunately, it's a very new component, and the documentation for it leaves us a few blanks to fill in.

I've home baked a solution that sort of uses this component, but also sort of circumvents it. I know there's likely a better way to do this, but for the moment I'm satisfied with this screen. It could still use a lot of love, such as animations or some navigation sound effects, and definitely some new art. But it's functional enough that I can proceed from it and focus on making a really satisfying gameplay loop for you.

## Working Around COVID-19
We all know these are uncertain times, and conducting business during the Coronavirus pandemic certainly is not business at usual. We wanted to let you all know that we're collaborating remotely and complying with government health policy. I mean, we can't really afford real estate right now, so it's not like there's an office to share anyway. But regardless, we're keeping safe and sincerely hope you're able to too.