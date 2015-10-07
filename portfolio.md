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
	        <image src="{{ site.baseurl }}{{post.avatarurl}}" style="height:300px"/>
	  	</li>
	{% endfor %}
</ul>