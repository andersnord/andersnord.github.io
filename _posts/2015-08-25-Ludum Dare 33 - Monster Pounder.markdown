---
layout: post
title:  "Ludum Dare 33 - Monster Pounder"
date:   2015-08-25 18:28:36
categories: jekyll update
tags:
- Unity
---

<a href="{{ page.url }}">
	<img src="{{ site.baseurl }}/assets/portfolio/monsterpounder/monster2.gif"/>
</a>

Monster Pounder is a game that I made together with [Zack Wood][ZackWebPage] for the **[Ludum Dare 33][LudumDare]** Game Jam, where the theme was "You are the monster". [Zack Wood][ZackWebPage] created the lovely running animation whereas I programmed and added everything inside Unity. Different sounds are played when the blocks are activated and when the orange guys are hit.

The core game idea is that each block represent a key on the keyboard. When a key is pressed, the corresponding block lunges out. The running orange guys are trying to get from the left side to the right side. The players mission is to pound them down before doing so.

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/monsterpounder/qwerty.gif" height="200px">
  <figcaption> QWERTY being pressed. Nordic ISO layout. </figcaption>
</figure>

What I like most about this idea (apart from being fun) is that it could potentially be used as a typing learning tool for educational purposes. 

#### Implementation ####

The game was implemented in Unity as a proof of concept. It took about 6 hours.

#### Images ####

<style>
	ul#menu li {
		float: left;
	    display:inline;
	    margin: 10px 10px 0 0;
	}
	ul#menu {
		margin: 0 0 0 0;
	}
	div.img li {
		height: 230px;
		width: 230px;
		overflow: hidden;
	}

	div.img img {
		max-height: 100%;
		max-width: 100%;
	}
</style>

<div class="img">
	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/monsterpounder/1.png">
			<img src="{{ site.baseurl }}/assets/portfolio/monsterpounder/1.png"/>
		</a>
		</li>
	  	<li><a href="{{ site.baseurl }}/assets/portfolio/monsterpounder/4.png">
			<img src="{{ site.baseurl }}/assets/portfolio/monsterpounder/4.png"/>
		</a>
		</li>
	  	<li><a href="{{ site.baseurl }}/assets/portfolio/monsterpounder/3.png">
			<img src="{{ site.baseurl }}/assets/portfolio/monsterpounder/3.png"/>
		</a>
		</li>
	</ul>
</div>

[ZackWebPage]:      http://wzackw.com
[LudumDare]: 		http://ludumdare.com/compo/ludum-dare-33/