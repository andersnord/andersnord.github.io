---
layout: page
title: Portfolio
permalink: /portfolio/
---

<ul class="post-list">
	{% for post in site.tags.portfolio %}
	 	<li>
	 		<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
		 	<h2>
		        <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
	        </h2>
	        <a href="{{ post.url }}">
	        	<image src="{{ site.baseurl }}{{post.avatarurl}}" style="max-height:200px; max-width:100%;"/>
	        </a>

	  	</li>
	  	<br>
	{% endfor %}
</ul>