---
layout: default
title: "Shoot Your Friends - First Week Down"
date: 2020-05-08 05:00:00 +0200
published: 2020-05-08 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends]
github: "https://github.com/zmalexander/"
noimage: true
---

# First Week Down
Hey friends, welcome to the Shoot Your Friends development diary!
<!--more-->
All too often we've been burned by video games where the developers do not make an effort to engage with the community and let us know what's going on. Can we expect new features soon? Is the game in development hell? Have they seen my fanart? These are all questions that we'd never get answered from uncommunicative developers - and that's something that we at Shoot Your Friends never want to be.

Before you start sending us fanart, you might want to know what this project is all about. Shoot Your Friends is a local multiplayer video game where you... shoot your friends. It's intended to be a couch game, something dear to the development team, with a fast gameplay loop and satisfying visuals. It's the perfect sort of thing for parties, if your parties are groups of 2-4 people who like shooting each other.

So check out this space for weekly updates on what we're working on. It's still really early in the development cycle, in fact probably too early to have anything exciting to share with you. But we've never done this before and want to get in the habit early. Plus we find the work we're doing interesting, so maybe somebody will nerd out with us.

## Who We Are
So you might be wondering who the heck are these guys even? Without getting too introspective, we're not too sure of that ourselves. It's so early in the development cycle that we haven't had nailed down a business name or jumped through all the hoops to become an incorporated entity. In fact, if you're reading this post when it was written, you're probably on one of our developers' personal GitHub pages right now.

So if we can't tell you about the company - since it doesn't exist - we can at least tell you about our operations. We're developing this game in Canada, in the east-coast province of New Brunswick. Most of us met in college, became firm friends, and started playing video games together. It wasn't long before we decided we ought to be building games too, seeing as how we have that skillset and all.

### Peter Adam
Hi, my name is Peter and I'm the lead developer for Shoot Your Friends. I have three years of experience with enterprise programming and close to three decades of experience with playing video games. I made my first game when I was eleven, and it's always been a hobby of mine since.

Apart from video games, I'm also into board games and roleplaying games. I've been a Game Master for tabletop games for about ten years now. On the Dungeons & Dragons / Pathfinder divide I usually responded with "either," or "both," but I've also dabbled in other games like Apocalypse World or Ironsworn. My all time favorite board game is Betrayal at House on the Hill, and that's probably in large part due to my love for cheesey movies. 

### Zach Mackay
Hey I'm Zach, and I'm the developer working on the UI portion of Shoot Your Friends while also helping out where I can. I have two years of programming & development experience, with five years of business & public relations experience. 

I have wildly varied interests, from playing video games, roleplaying games, website development, programming, photography, hiking, exploring cities, business PR, online sales, investments, real estate, working out, yoga, minimalism, travelling the world, psychology, gardening, scuba diving, skydiving, and an ambition that keeps me constantly learning new things. I am the person who will try anything at least once!

I put together the blog for Shoot Your Friends with efficiency in mind, and I am successful! The blog is low cost (free) & low maintenance once set up, and posting is just as easy as using WordPress. While there's always improvements to be made to the blog, I'm happy with the progress made so far.

If you want to know more about me, check out my website and portfolio here - <a href="www.zachmackay.com">zachmackay.com</a>.

### Sara Ring

### Gerry Vautour
Hi there. I'm Gerry, another developer on Shoot Your Friends. I dropped out of a programming course in college, missed it, and when these guys suggested we make a game together, I immediately jumped on board. I've played games my whole 30-some years of life, and have always wanted to spend my time making games but had no clue where or how to start.  Now I have some knowledge, and a group to help keep me on track.
I'm not the social type, so you likely won't hear much from me on a regular basis. I'll just be working in the background to make the best games I can, and hopefully someone out there will like them.

## Pregame Lobby
Arguably, one of the first things a player will do when they start the game is try to start the game. We think this is a fair and justified response, and take our players to the pregame lobby. This is a screen that's probably familiar to you, where each player pushes a button on their gamepad to enter the game.

<img class="center-block img-responsive" src="/assets/images/{{page.id}}/lobby5.gif" alt="Image description here"/>

This screen has a surprising amount of complexity to it. Each player is going to use a different gamepad. They might decide to back out after they've started so they can change their avatar's skin. Controllers might get swapped out when your host gives you a knock-off controller. Fortunately, our engine (Unity - for anybody curious) has a new component that helps us keep track of which players belong to which controllers. Unfortunately, it's a very new component, and the documentation for it leaves us a few blanks to fill in.

I've home baked a solution that sort of uses this component, but also sort of circumvents it. I know there's likely a better way to do this, but for the moment I'm satisfied with this screen. It could still use a lot of love, such as animations or some navigation sound effects, and definitely some new art. But it's functional enough that I can proceed from it and focus on making a really satisfying gameplay loop for you.

## Working Around COVID-19
We all know these are uncertain times, and conducting business during the Coronavirus pandemic certainly is not business at usual. We wanted to let you all know that we're collaborating remotely and complying with government health policy. I mean, we can't really afford real estate right now, so it's not like there's an office to share anyway. But regardless, we're keeping safe and sincerely hope you're able to too.
