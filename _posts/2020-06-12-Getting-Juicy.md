---
layout: default
title: "Getting Juicy"
date: 2020-06-12 05:00:00 +0200
published: 2020-06-12 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends,juice]
github: "https://github.com/zmalexander/"
noimage: true
---

# Getting Juicy
Hello friends! Welcome back to another week in our development diary. Today I wanted to talk about juice.
<!--more--> 
And that's not apple, orange, or some healthy blend of quinoa and kale. Juice is a term in the game development community that refers to how the game feels to play it. Generally, people want to play juicy games, but sometimes we struggle to define exactly what makes it so. 

Well, we've been hard at work trying to infuse some more juice into Shoot your Friends, and we've got to say that the game looks about a zillion times better as a result.

## Bullet Trails
The core mechanic of Shoot your Friends is the ability to shoot your friends. Previously, we were using sad, whimpy bullets suitable for sad, whimpy people. They were a static image of a rounded square with no pizzazz or oomph applied.

<img class="center-block img-responsive" src="/ShootYourFriendsWebsite/assets/images/{{page.id}}/bullets.gif" alt="Bullets with colourful trails"/>

Enter pizzazz and oomph. We've updated the sprite, added some trails, and keyed those trails to match the player's team colour. A lot of our design is influenced by 80's Outrun aesthetic, and what could be more 80's than neon? So we took a look at neon lights and modeled our bullets to be reflect that.

## Updated Tilemaps
<img class="center-block img-responsive" src="/ShootYourFriendsWebsite/assets/images/{{page.id}}/new-floors.png" alt="A new tilemap showing a wireframe floor"/>

Previously, our levels used dull background colour to resemble a floor. We've decided to jazz that up by introducing a tilemap to them. Currently this tilemap targets the floor, but we're looking to do something similar for our walls which are currently still using a placeholder tilemap.

## Dodge Cooldown
In response to our testers' feedback, we wanted some way to visually show the player that their dodge roll was off cooldown. Previously, you just had to know when it was ready, and count the seconds between dodges. Counting is for nerds, so our thought was to add a little progress bar under the player to show when it was recharging.

<img class="center-block img-responsive" src="/ShootYourFriendsWebsite/assets/images/{{page.id}}/dodge-bar.gif" alt="A little whoopsie with our dodge bar"/>

Gerry worked hard to introduce our dodge bar, and he got it in the end. But he thought this interaction was hilarious and wanted to show it off.

## User Interfaces
In response to our art director's feedback, we've updated our user interface. We used to put everything together with a devil may care attitude and hoped our players wouldn't notice. Now we're working to bring a more unified look to the each menu. Here's a before-and-after of our start menu:

<img class="center-block img-responsive" src="/ShootYourFriendsWebsite/assets/images/{{page.id}}/title-screen-before-after.png" alt="The title screen before and after visual improvements"/>

## Taking Care of Business
This past week we've been talking with lawyers, accountants, and people who are generally more grown up than we are. The result of these meetings is that it won't be too much longer before we have a bona fide business

All of this means that we're one step closer to being able to release. I don't want to talk about a release date yet though. We've seen the game requires some more polish anyway, and we still haven't really looked at marketing or anything like that ahead of the release cycle. But the needle's shifted from "maybe" to "sometime," and that's cause for excitement!
