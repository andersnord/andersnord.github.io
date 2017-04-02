---
layout: post
title:  "Synaptics - Touchpad integration"
date:   2015-11-01 09:28:36
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

The touchpad features start at 1 minute and 36 seconds.

<iframe width="560" height="315" src="https://www.youtube.com/embed/SYwd9Lt1ve4" frameborder="0" allowfullscreen></iframe>

## Implementation ##
- C#
- C++
- Synaptics API.

[TobiiTech]: http://www.tobii.com/tech/
[TouchpadInstructionVideo]: https://www.youtube.com/watch?v=SYwd9Lt1ve4&t=95s
[SynapticsReveal]: http://www.tobii.com/group/news-media/press-releases/tobii-and-synaptics-unveil-concept-laptop-that-integrates-eye-tracking-and-touchpad-user-interface-controls/