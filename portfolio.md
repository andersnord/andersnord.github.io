---
layout: page
title: Portfolio
permalink: /portfolio/
---

<ul>
	{% for post in site.tags.portfolio %}
	 	<li>
	        <a href="{{ post.url }}">{{ post.title }}</a>
	        <span class="date"> -  {{ post.date | date: "%B %-d, %Y"  }}</span>
	        <br>
	        <a href="{{ post.url }}">
	        	<image src="{{ site.baseurl }}{{post.avatarurl}}" style="height:200px; max-width:100%;"/>
	        </a>
	  	</li>
	  	<br>
	{% endfor %}
</ul>