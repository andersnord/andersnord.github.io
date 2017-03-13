---
layout: post
title:  "Synaptics - Touchpad integration"
date:   2017-02-01 09:28:36
categories: jekyll update
avatarurl: /assets/portfolio/tobii/synaptics/Synaptics_logo.png
tags:
- portfolio
- C#
---

<a href="{{ page.url }}">
  <img src="{{ site.baseurl }}/assets/portfolio/tobii/synaptics/Synaptics_logo.png" />
</a>

When I was working at [Tobii][TobiiTech] I was the main developer for an [Alienware][Alienware] integration specific feature called keyboard light. What it did was letting you control their keyboard light feature with your eyes. So when looking at a certain region of your keyboard, it would light up. This saves energy as well as being conveinient when working in the dark for example. It is also a cool gimmick for gamers.

We integrated the Tobii desktop software with their keyboard light API to be able to communicate between the different softwares.  

# Keyboard Light press release: #
> Now equipped with the ability to understand the user’s current focus and attention, the Alienware 17 is able to optimize the power exchange between both the keyboard’s lighting zones and the screen. When the user is looking at the screen the keyboard backlights remain off since the user is not currently interested in this area. Key illumination also only occurs in the region the user is currently looking, rather than the entire keyboard, further optimizing power management

I also prototyped the [Wake On Gaze][Alienware] feature.

# Wake On Gaze press release: #
> In order to wake the notebook up from sleep mode, the user looks directly at the Alienware logo and the device will power up. This ensures the notebook acts on the specific user intent of activating the device and avoids accidental power ups. 

## Implementation ##
- C#
- Alienware Keyboard Light API.

## Keyboard Light in action ##
<figure>
  <img src="{{ site.baseurl }}/assets/portfolio/dimensionshift/livegameplay.gif"/>
  <figcaption> First level </figcaption>
</figure>

## Images from project ##
<div class="postimages">
  <ul>
    <li><a href="{{ site.baseurl }}/assets/portfolio/dimensionshift/Dots.png">
      <img src="{{ site.baseurl }}/assets/portfolio/dimensionshift/Dots.png"/>
    </a>
    </li>
        <li><a href="{{ site.baseurl }}/assets/portfolio/dimensionshift/Rectangles.png">
      <img src="{{ site.baseurl }}/assets/portfolio/dimensionshift/Rectangles.png"/>
    </a>
    </li>
        <li><a href="{{ site.baseurl }}/assets/portfolio/dimensionshift/Cube.png">
      <img src="{{ site.baseurl }}/assets/portfolio/dimensionshift/Cube.png"/>
    </a>
    </li>
  </ul>
</div>

[Alienware]: http://www.tobii.com/group/news-media/press-releases/2016/9/alienware-creates-worlds-first-intelligent-notebook-with-tobii-eye-tracking/
[TobiiTech]: http://www.tobii.com/tech/
[SynapticsReveal]: http://www.tobii.com/group/news-media/press-releases/tobii-and-synaptics-unveil-concept-laptop-that-integrates-eye-tracking-and-touchpad-user-interface-controls/