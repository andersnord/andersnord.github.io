---
layout: post
title:  "Game development - Teaching the player - Part 1: Input"
date:   2016-11-07 10:28:36
categories: jekyll update
tags:
- Game Development
---

- Discovering the controls and core mechanics
- left, right
- jump
- walljump
- Energy cubes

För och nackdelar. 
Hur jag kom fram till att behålla walljump och att ändra kuberna från att göra inget till att ändra på protagonisten.

This post will try to explain the process of discovering the controls and core mechanics. I wanted to divide them into separate posts, but since they are so tightly coupled it does most sense to explain them together. 

# Introduction #

I had some initial thoughts about the controls and how they were supposed to feel. I wanted them to be very responsive and predictable. The player should not have to worry about stepping over a ledge because of slippery controls. Rather, they should be able to focus on the level and how to traverse it in the best possible way.

## Controls ##

# Inital controls #
In the initial version it was possible to move left, right and jump ( analog ). It was then possible to jump heigher by holding the jump button ( analaog ) and run faster by holding the run button ( digital ). It was also possible to walljump by moving the protagonist against the wall and jump.

* GIF showing text above *

# Final controls #
In the final version it is possible to move left, right and jump ( digital ). It is no longer possible to jump different heights or run faster by holding any button. Instead the energy cubes ( core mechanic, see below ) can alter the speed an jump height of the protagonist. 

* GIF showing text above *

## Core Mechanics ##

# Inital mechanics #
- Energy cubes ( without ant altering powers )
- Walljump
- Returning to ship.

# Final mechanics #
- Energy cubes ( Alternated )
- Walljumps ( Stayed the same )
- returning with cube to ship ( Removed ) - backtracking.

- according to keep it simple. Rather cut away stuff.

## The path down discovery road ##
So why did I make these changes? And how did I motivate them? (Rätt ordval?) 
First of all, I started testing early and often. With a wide range or personalities and type of gamer. By doing so I could quickly recognize the obvoius flaws and unnecessary things in the game. I will try to categorize them below.

# Energy cubes vs speed and height #

# Returning to the ship #

# 




Förklara hur jag gick till väga när jag valde kontrollerna.

- Testade och såg reaktionerna.
- Gillade ej backtracking.
- 



# Final #

Some early prototype controls / mechanics:

- Show GIF with shooting and double jump -







## Teaching the controls and core mechanics ##
- Level design
- Visual feedback



# Introduction #
 Also I wanted to be able to explain the controls without any text-tutorials, but with pure level design. Also I tried to make all the decisions based on the fact that I am supposed to do everything by my self. Programming, grahpics and art, level design, sound and music and so on. So I really wanted to keep things as simple as they could be.

----

 To learn the player what they are able to do with the protagonist, there are a couple of different parts that combined gives the player this knowledge. I have so far tried to stay away from sound too much visual feedback. This is due to my hypotheses: If I can teach the player the controls and core mechanics of the game when using simple graphics and no sound, then more people will get it once they are added.

----

I created a prototype with the controls that I liked and then let people play it. I tried not to say anything and see what they did. This was the most valueable thing. It beats all other testing in my opinioon. You can see how the tester is reacting and what they get stuck on, for how long, if they are having fun, and the list goes on. I also notes all the feedback I got and tried to evaluate it afterwards.

----





Att ha med som GIF:
- TLP Ver 2: Visa hur mycket man blev påverkad av kuberna. Dock mer för energy-cubes. Så ej denna versionen.
- ROF - Visuella effekter (men man fattade knappt ändå, förrutom jump)
DONE - ROF - där man kunde springa och hoppa högt.
DONE - ROF - Double jump - Ej ha med för va så kort period det var intressant. Kan nämna det. 
DONE - ROF - Shooting (Med physics kanske?) - X ha inte med tror jag. För random. Kan nämna.
DONE - ROF - Jumping height, analog + Digital (För att inte ha för många videos)
DONR - ROF - Hard to control in air
 - TLP - Easier to control in air
- TLP - Different player states.
- ROF - Speed-button.

*Picture of Half double jump, half normal jump* (Hmm..)

This post will be about how the final controls was found, how we teach them to the player and the reasoning behind using them instad of the initial controls.

# Introduction #

Some information before we start. I had some initial thoughts about the controls and how they were supposed to feel. I wanted them to be very responsive and predictable. The player should not have to worry about stepping over a ledge because of slippery controls. Rather, they should be able to focus on the level and how to traverse it in the best possible way. Also I wanted to be able to explain the controls without any text-tutorials, but with pure level design. Also I tried to make all the decisions based on the fact that I am supposed to do everything by my self. Programming, grahpics and art, level design, sound and music and so on. So I really wanted to keep things as simple as they could be.

* GIF of Digital jumping + analog with effects *
- One of the earlier verions where jump had an analog aspect -

# Teaching the player #

To learn the player what they are able to do with the protagonist, there are a couple of different parts that combined gives the player this knowledge. I have so far tried to stay away from sound too much visual feedback. This is due to my hypotheses: If I can teach the player the controls and core mechanics of the game when using simple graphics and no sound, then more people will get it once they are added.

* GIF of Walking -> Running with effects *
- When you needed to hold a button to run -

I created a prototype with the controls that I liked and then let people play it. I tried not to say anything and see what they did. This was the most valueable thing. It beats all other testing in my opinioon. You can see how the tester is reacting and what they get stuck on, for how long, if they are having fun, and the list goes on. I also notes all the feedback I got and tried to evaluate it afterwards.

* GIF of hard to control in air *
- When air control was too sensitive -

So in the initial - initial version, it was possible to double jump and shoot cannon balls to the left and right. Lets call this the prototyping phase. In the initial version (where we will start) it was possible to move left, right and jump. It was then also possible to jump heigher by holding the jump button and run faster by holding the run button. This can be seen in the GIF´s Above.

These controls were hard for people to grasp, since there was no literal explanation. Even with the visual effects and level design it was hard. Also, I noticed that people tend to always hold the run button and always hold the jump-button for the maximum amount of time. They rarely understood in the end that it was possible to jump different heights. This was ofcourse partly my fault. But when I tried to do explain this through level design, people still did not fully understand. So what this told me was that it did not feel natural to, mostly, casual players, to hold the jump-button for different heights.

And since I wanted to keep it simple and did not see any loss for the game idea, i dropped the analog part of the jump. Now you always jump the same heigt, no matter how long you press the jump button. Also I would replace the higher jump with jump-energy cubes.

* GIF - Digital jump *

I did the same thing for the running part. Now there is only one current speed, which the speed-energy-cube can alter permanently.

* GIF - Runnin Quicker with cube *
* GIF - Jumping height with jump-cube *
- ta från post 1 kanske -

Also the air control was really hard to get right, and as I mentioner in the beginning, I prioritized that there should not be a problem with the controls. So I basically made aircontrol a little slower(accelerate slower).

* GIF - Air control *

# Why start with controls? #

One idea behind doing the controls first was that I wanted to be able to start creating levels. And I did not want to change them later due to changes in the control-scheme. Also the effects of the cubes. On jump cube would make you jump a certain amount higher. And since you can only jump one digital height, this palys into how sensitive the levels are to that.



# Final #
I hope this shed some light into the process of how I got the correct controls. Until next time, I am going to leave you with some control-features that never made it into the game.

- GIF of shooting
- GIF of double jump
- GIF..


So to the inital input. The control scheme was:
- Double jump
- Shooting right and left
- Possible to double jump very high due to adding force.
- Dying - Colors on player show health (dead space).
- Jumping higher by holding down jump-button
- Super hard to control in air (and on ground) - From playing now - Irritating dying each time.
- Added Visual feedback from dying(blood), from explosion, Jumping, Energies teleporting. Holding down jump.
- Added Color for different player states.
- Digitala hopp. Och Run gör att du hoppas högre. (2 Digitala hopp.)
- Digitalt hopp + analogt (SMB)
- 0 friktion när man sprang.

- Added rolling - Possible to climb and does not have to jump.

# Changed #
- From having lives -> Die instantly -> Cannot get killed. -- Frustration and complexity.

# Removed first #
- Double jump
- Added speed button.


- Controls and how they were prototyped from first version.
Hur jag levt efter quoten "Less is more"-ish.



- 







<img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/header.png"/>

Hello, and welcome to a series about Indie Game Development. These posts will contain everything that occurs when developing an indie game as a single person.

So this first post will be an introduction to what kind of game I am developing and some information around it. 

I have been working on this game during weekends since the beginning of 2015. Since three weeks back I have started working 60% on it while working 40% at my regular job. This means 3 days a week which hopefully is enough to finish this project within a reasonable time frame. This is something I will talk about in a later post (scoping). And if it has not been clear, the game is still in a prototyping phase where the main controls and main gameplay mechanics are pretty much done. But graphics, level design and sound are still distant.

## About the game ##

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/PhysicsAndState.gif"/>
  <figcaption>Physics impact on gameplay.</figcaption>
</figure>

# Story #
It all starts with the protagonist having to do an emergency landing on a foreign planet. To be able to continue their journey, they have to collect radioactive energy. The energy puts the protagonist in tremendous pain but is a necessary sacrifice to be able to return home. It also alters and enhances the protagonists abilities permanently until the space ship can harvest the energy and releive them from the pain. Which makes each level a new start, ability-wise.

The theme of the game is set in space and will include different planets. So I am hoping to be able to vary the environments quite a bit.

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/SpeedStompers.gif"/>
  <figcaption>Energy altering the speed of the protagonist.</figcaption>
</figure>

# Gameplay #
The game is a 2D platformer with puzzle elements. The platforming part is a mix between straight forward twitch reflex platforming and more casual super mario bros platforming. The puzzle part is divided into several components. One part consists of combining the different energies in the correct order to solve how to get them all. The goal for each level is to collect enough energy for your spaceship to be able to travel to the next level. The levels will include things like:
- Enemies, both dynamic and static ones.
- Physics based interactions, like jumping springs, buoyancy effects, wind, gravitation-less platforms, surface friction and more.
- Different environments that affects how the player must consider its options.

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/JumpEnergy.gif"/>
  <figcaption>Energy altering the jumping height of the protagonist.</figcaption>
</figure>

# Features #
- It is a 2D platformer set in a 3D environment.
- It is a mix between a platformer and a puzzle game.
- The collected energy follows the protagonist and can be used for physical interactions.
- The collected energy permanently alters the ability of the protagonist until the level is completed.
- Realistic physics affecting the protagonist.

## Final ##
I hope you will follow my journey and just drop me an email if there is anything you would like to know. Until next time, take care!

# Early game screenshots #

<div class="postimages">
	<ul>
		<li><a href="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/1.png">
			<img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/1.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/2.png">
			<img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/2.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/3.png">
			<img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/3.png"/>
		</a>
		</li>
	</ul>
</div>