---
layout: default
title: "Our Very First Build - Pre - Alpha"
date: 2020-05-29 05:00:00 +0200
published: 2020-05-29 05:00:00 +0200
comments: true
categories: development
tags: [gamedev,multiplayer,shootyourfriends]
github: "https://github.com/zmalexander/"
noimage: true
---

# Our Very First Build
Hello friends! We're very excited to announce that we've finished our first build of Shoot your Friends.
<!--more-->
It's in a rough state, and there's some bugs that render it unplayable, but like with your cousin's ugly baby you get this weird sense of pride and accomplishment to go with it.

When we set out to build this game, we started with the very ambitious goal to crank out our prototype in a month. It was a bumpy ride - so bumpy we didn't manage to keep up our blogging commitments. Sorry about that! We learned a lot along the way though, and it'll make things better for next time.

You might be wondering what's in this build. Well, you can start a game, select a colour for your players, and play a quick round by shooting your friends. It doesn't sound like much, but this past month has been a roller coaster. We'd be remiss if we didn't share what we learned along the way.

## It Takes Longer Than you Think
I'm no stranger to the internet. I play my video games online and I check in with their communities. One thing I see all the time is when there's some lacking feature or quality-of-life improvment there's always some disgruntled players pointing out how it'd take a day to fix. I usually laugh when I see this, because I know that programs have a way of becoming tangled and it always takes longer than they think. So knowing that, I went into this game with the expectation that things are going to take a long time.

And they took longer than that.

Part of why things took so long was that we didn't spend a super long time in the conceptual phase. Shoot your Friends is a simple concept - after all - and ultimately we underestimated its complexity.

The software leads follow the maxim *move fast and break something*, and it showed. There's pros and cons to this approach, of course. We broke stuff, but we hit our deadline. Sure, the broken stuff still needs fixing, and it's really damaging to the enjoyment of this game if we left them in their current state. But I'll sleep better at night knowing we hit our goal than if we had a flawless game that was only 10% done in this time.

## New isn't Always Better
By trade I'm a programmer, and when I have a new project I get this compulsion to try out a new framework because it supposedly makes my life easier.

Early in this last month, I pushed hard for us to use a brand spanking new component for Unity. This was the Input System, which is positioned to replace the Input Manager. And oh, what a component it is. It promises a complete rewrite of how we get input from the players, a more intuitive callback-based system for actions across multiple controller schemes, and - importantly for us - greatly simplifies handling multiple players locally. Sounds great, right?

It was a total dumpster fire.

Input System was released about a week before we started our project, as opposed to the Input Manager which I've pegged for release somewhere around 2011. This meant Unity has had almost a decade to round out documentation on it, and its community has had that time to build countless tutorials and Q&A's over common pitfalls. That support network just can't exist for something so new, which was a hard lesson for us to learn.

Ultimately, we had to shelve the Input System for our project. It was just impossible for us to tell if our bugs were a problem with the component or (more likely) our implementation. That said, I'm keeping an eye on this feature for the future. What worked great for the Input System really did work terrifically, and in a few years time I'm sure it'll have that support network we so desparately needed.

## What's Next?
We've decided that our developers have earned some rest and relaxation. So for the next week we expect to be focused on the administrative stuff that doesn't make for a compelling development diary. When we do get back to the game, it'll be for some much needed polish and bug fixing.