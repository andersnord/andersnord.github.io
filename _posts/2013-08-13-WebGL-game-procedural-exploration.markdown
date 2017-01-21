---
layout: post
title:  "Procedural exploration"
date:   2013-08-13 18:28:36
categories: jekyll update
avatarurl: /assets/portfolio/proceduralexploration/procedural_main.png
tags:
- school
- portfolio
- webgl
- javascript
---


<iframe src="http://player.vimeo.com/video/75006612?color=4B0082" width="100%" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe> 


In this project a procedural simplex noise function is implemented in a WebGL game.

#### Implementation ####

the game was implemented in WebGL. WebGL communicates with the graphics-card through OpenGL ES 2.0-standard shaders. To access these in html, javascript is being used. The matrix library used was glMatrix v0.9.5.

## [Report][ProceduralReport] ##

#### Images from project ####

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
		<li><a href="{{ site.baseurl }}/assets/portfolio/proceduralexploration/player_view.png">
			<img src="{{ site.baseurl }}/assets/portfolio/proceduralexploration/player_view.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/proceduralexploration/player_view_dead.png">
			<img src="{{ site.baseurl }}/assets/portfolio/proceduralexploration/player_view_dead.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/proceduralexploration/above_hit.png">
			<img src="{{ site.baseurl }}/assets/portfolio/proceduralexploration/above_hit.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/proceduralexploration/cube_light.png">
			<img src="{{ site.baseurl }}/assets/portfolio/proceduralexploration/cube_light.png"/>
		</a>
		</li>
	</ul> 
</div>

[ProceduralReport]: /assets/portfolio/proceduralexploration/Report_andno922_TNM084.pdf