---
layout: post
title:  "Synaptics - Touchpad integration"
date:   2015-06-01 09:28:36
categories: jekyll update
avatarurl: /assets/portfolio/tobii/synaptics/Synaptics_logo.png
tags:
- portfolio
- C#
---

<a href="{{ page.url }}">
  <img src="{{ site.baseurl }}/assets/portfolio/tobii/synaptics/Synaptics_logo.png" />
</a>

When I was working at [Tobii][TobiiTech] I was one of the main developers for integrating the synaptics touchpad API with our software. This included analyzing their bitstreams and figure out how to create a system that recognized what type of finger motion the user was trying to do.

Usage examples are:
- Scrolling at the position where you are looking when doing a two finger draging motion.
- Teleporting the cursor to the position where you are looking when putting the finger down on the touchpad.
- Zooming at the position where you are looking when pinching.

## Implementation ##
- C#
- C++
- Synaptics API.

## Reviwer showing features ##
<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/dimensionshift/livegameplay.gif"/>
</figure>

[TobiiTech]: http://www.tobii.com/tech/
[SynapticsReveal]: http://www.tobii.com/group/news-media/press-releases/tobii-and-synaptics-unveil-concept-laptop-that-integrates-eye-tracking-and-touchpad-user-interface-controls/