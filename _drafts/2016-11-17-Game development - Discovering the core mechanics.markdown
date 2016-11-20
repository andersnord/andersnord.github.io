---
layout: post
title:  "Game development - Discovering the core mechanics"
date:   2016-11-17 09:28:36
categories: jekyll update
tags:
- Game Development
- Unity
---

* Image*
<img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/header.png"/>

This post will try to explain the process of discovering the core mechanics. If you havent read the previous post, please do so before continuing.

# Introduction #

Förklara lite kring hur jag ville hålla core mechanics. Simple osv men unika osv.

## Core Mechanics ##

# Inital mechanics #
- Energy cubes -
The goal of the game was to collect energy cubes and return them to the ship. They followed the protagonist without affecting them.

* GIF showing text above *

- Walljump -
The protagonist was able to walljump. Both upwards one wall, or between two.

* GIF showing text above *

- Returning to ship -
The energy cubes needed to be returned to the space ship. The space ship was also the starting point of the current level.

* GIF showing text above *

# Final mechanics #
- Energy cubes ( Altered )
In the final version, the energy cubes altered the protagonists abilities permanently in different ways.

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/1_Introduction/JumpEnergy.gif"/>
  <figcaption>Energy altering the jumping height of the protagonist.</figcaption>
</figure>

- Walljumps -
These are kept pretty much as they were with some minor changes to improve the user experience.

- returning with cube to ship ( Removed ) -
This feature was cut out due to the fact that it promoted backtracking for every level.

## The path down discovery road ##
So why did I make these changes? And how do I motivate them? 
First of all, I started testing early and often. With a wide range of personalities and gamer-types. By doing so I could quickly recognize the obvoius flaws and unnecessary things in the game ( things that did not directly contribute to the core ideas ). I will to categorize them below. 

# Energy cubes #
The initial version of cubes just followed the player when collected. They could be physically interacted with. To push enemies away, but also to be in the way when jumping. This behaviour has not changed. But I felt that there was something missing here. And when I removed the extra buttons for jumping heigher and running faster, it clicked. Now the energy cubes can alter the jump height and speed of the protagonist, permanently. They can also alter other things, but thats for another post.

# Returning to the ship #
From the beginning, the collected energy cubes needed to be returned to the space shipt. The space ship was the starting point. Visually and story-wise, this did make a lot of sense. Return energy to the space ships empty tanks to be able to continue. But what this did was introduce backtracking into every level. Not very good, right? So to solve this, I basically removed the visible space shipe. Now you just have to collect a set number of energy cubes before completing the level. In the current state the level just completes, but in the future there will be a beam appearing from the sky. walking into this one will return the protagonist to the space ship.

# Walljumps # 
People found this interaction fun and they all seemed to graps the interaction quickly. The only part I had to alted was setting a timer before leaving the wall. This would prevent the protagonist to fall from the wall before the player has had time to push jump.

# Final #

Some early prototype mechanics:

- Show GIF with first prototypes. Different effects from cubes -

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