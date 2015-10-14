---
layout: post
title:  "Light WebGL Engine"
date:   2013-08-13 18:28:36
categories: jekyll update
avatarurl: /assets/portfolio/webglengine/ver9.png
tags:
- school
- portfolio
- Javascript
- GLSL
---

<iframe src="http://player.vimeo.com/video/75006611?color=4B0082" width="400" height="225" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe> 

The goal with the project was to implement a simplistic game in WebGL. It somewhat became more of a simple game-engine.

#### Implementation ####

The game engine was implemented in WebGL using shaders. WebGL communicates with the graphics-card through OpenGL ES 2.0-standard shaders. To access these in html, JavaScript is being utilized. The matrix library used was glMatrix v0.9.5.

## [Report][EngineReport] ##

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
		<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/ver9.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/ver9.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/depthtexture.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/depthtexture.png"/>
		</a>
		</li>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/pixel_shading.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/pixel_shading.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/specular.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/specular.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/lightshadow.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/lightshadow.png"/>
		</a>
		</li>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/w_perspective.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/w_perspective.png"/>
		</a>
		</li>
	</ul> 

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/wo_textures.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/wo_textures.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/webglengine/bounding_real.png">
			<img src="{{ site.baseurl }}/assets/portfolio/webglengine/bounding_real.png"/>
		</a>
		</li>
	</ul> 
</div>

[EngineReport]: /assets/portfolio/webglengine/Report_Anders_Nord-DVGB06.pdf