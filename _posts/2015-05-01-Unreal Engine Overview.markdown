---
layout: post
title:  "Unreal Engine 4 - Basic map creation"
date:   2015-08-25 18:28:36
categories: jekyll update
tags:
- Unreal Engine 4
- Blender
---

<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/11.png">

To get a general understanding of Unreal Engine 4 I decided to create a battleground map with some basic game mechanics. I used as many tools in the editor as possible to get a good understanding of what UE4 offers and what it can achieve.

The final result ended up being a battleground map where you control a spider character that aligns to the surface. You can also jump into the spinning cubes to make them explode.

This project aslo made it possible for me to create some basic 3D models and animations with Blender, which can be seen throughout the map.

#### The Blueprint System was used for: ####

- Implementing the materials.
- Controlling the player (Keyboard and mouse).
- Animation states for the player when in idle and moving state.
- Logic for exploding cubes.
- Rotating spheres.

#### The C++ Scripts were used for:#### 

- Aligning the character with the ground.

The blueprint system is basically a node-graph where you can drag lines between different boxes. They allow non-programmers to create features on their own, a kind of visual scripting. This is primarily for designers (even though programmers might find it quicker for smaller tasks as well), but it is a good middle ground for letting designers and programmers co-operate. The C++ scripts are the more traditional way of coding the behavior.

### Map overview - High resolution images at the bottom ###

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/GIF/OverviewFlyingTrimmed.gif" height="250px">
  <figcaption> Overview of map. </figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/GIF/OverviewBottomTrimmed.gif" height="250px">
  <figcaption> Player running through the bottom part of the map. </figcaption>
</figure>

### Specific game implementations ### 

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/GIF/SurfaceRotationTrimmed.gif" height="250px">
  <figcaption> Player is aligning with the surface. </figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/GIF/ExplosionTrimmed.gif" height="250px">
  <figcaption> The cube explodes when colliding with the player. </figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/GIF/Water2Trimmed.gif" height="250px">
  <figcaption> Water material affects the geometry of the mesh. </figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/GIF/SpinningBallsTrimmed.gif" height="250px"/>
  <figcaption> Spinning spheres. </figcaption>
</figure>

#### Implementation ####

This project was implemented using Unreal Engine 4. The Blueprint System as well as C++ Scripts has been used. Blender was used for creating the 3D models and animations.

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
		<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/1.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/1.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/2.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/2.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/3.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/3.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/4.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/4.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/5.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/5.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/6.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/6.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/7.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/7.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/8.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/8.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/9.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/9.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/10.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/10.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/11.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/11.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/12.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/12.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/13.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/13.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/unrealoverview/14.png">
			<img src="{{ site.baseurl }}/assets/portfolio/unrealoverview/14.png"/>
		</a>
		</li>
	</ul>
</div>

[ZackWebPage]:      http://wzackw.com
[LudumDare]: 		http://ludumdare.com/compo/ludum-dare-33/