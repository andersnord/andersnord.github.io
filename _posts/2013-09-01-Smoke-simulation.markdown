---
layout: post
title:  "GPU Smoke simulation"
date:   2013-09-01 18:28:36
categories: jekyll update
avatarurl: /assets/portfolio/smoke/fField_2.png
tags:
- school
- portfolio
- C++
- GLSL
---

<iframe src="http://player.vimeo.com/video/75007723?color=4B0082" width="100%" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe> 

This fluid simulation efficiently implements a method for simulating smoke entirely on the GPU. The model is unconditionally stable and produces complex fluid-like flows.

#### Implementation ####

This project has been implemented in programming language C/C++ on the GPU. This was achieved by using GLSL. API´s and librarys that has been used are the math library glm, the multi-platform library GLFW and graphics library OpenGL.

## [Report][SmokeReport] ##

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
	div.img img {
		height: 230px;
		width: 230px;
	}
</style>

<div class="img">
	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/fField_2.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/fField_2.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/fField_3.png">
		  		<img src="{{ site.baseurl }}/assets/portfolio/smoke/fField_3.png">
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/blacksmoke.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/blacksmoke.png"/>
		</a>
		</li>
	</ul>

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/layersmoke.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/layersmoke.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/dField_3.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/dField_3.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/pField_31.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/pField_31.png"/>
		</a>
		</li>
	</ul> 

	<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/vField_3.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/vField_3.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/smoke/fField_2.png">
			<img src="{{ site.baseurl }}/assets/portfolio/smoke/fField_2.png"/>
		</a>
		</li>
	</ul> 
</div>
[SmokeReport]: /assets/portfolio/smoke/Smoke_report.pdf