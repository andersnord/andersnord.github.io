---
layout: post
title:  "Game development - Discovering the controls"
date:   2016-11-20 09:28:36
categories: jekyll update
tags:
- Game Development
- Unity
---

<!--<object data="{{ site.baseurl }}/assets/GameDevelopmentPosts/2_Controls/controller.svg" type="image/svg+xml">-->
<a href="{{ page.url }}">
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/2_Controls/controller-640.png" />
</a>
<!--</object>-->

This post will try to explain the process of discovering the controls. I have divided controls and core mechanics into separate posts even though they are somewhat coupled. This is because I want to keep the posts short and focused.

# Introduction #

I had some initial thoughts about the controls and how they were supposed to feel. I wanted them to be very responsive and predictable. The player should not have to worry about stepping over a ledge because of slippery controls. Rather, they should be able to focus on the level and how to traverse it in the best possible way.

I started out by developing the controls because I wanted to finish them before continuing. This was due to the fact that all levels will depend heavily upon them. If they change later, a lot of things may break. A level is created and thought out with these exact controls in mind, so there is a clear symbiosis.

# Inital controls #
In the initial version it was possible to move left, right and jump. It was then possible to jump higher by holding down the jump button (analog) and run faster by holding down the run button (digital). Further it was possible to control the protagonist in the air.

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/2_Controls/InitialControls.gif"/>
  <figcaption>Initial controls.</figcaption>
</figure>

# Final controls #
In the final version it is possible to move left, right and jump (digital). It is no longer possible to jump higher or run faster by holding any button. Instead the energy cubes (core mechanic, see previous post, or next one) can alter the speed and jump hight of the protagonist. Air control still exists.

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/2_Controls/FinalControls.gif"/>
  <figcaption>Final controls.</figcaption>
</figure>

## The path down discovery road ##
So why did I make these changes? And how did I motivate them? 
First of all, I started testing early and often. With a wide range of gamer-personalities. By doing so I could quickly recognize the obvious flaws and the unnecessary - "does not contribute to the core ideas" - controls in the game.

# Discoveries #

In the initial version, people generally had a hard time discovering and understanding how pressing jump and run affected the protagonist. I tried explaining the controls through level design and visual effects. But none of these helped. My conclusion was that the those controls were too complicated for people to grasp instinctively.

- Running: I noticed that people tended to always press the run button or not discovering it at all. Because of this, I removed having two different speed-states. Now there is always only one current top speed. But there is some acceleration to make it easier to anticipate smaller movements.

- Jumping: The testers almost always pressed the jump-button for the maximum amount of time. Since it did not feel natural to most players to hold down the jump-button to reach different heights, I scrapped it and made it digital. Now the protagonist always jumps the same amount, independent of how long the jump button is pressed. This change was very noticable when looking at how quick the player learned when and how to jump.

- Air control: The acceleration curve was changed so that the player felt more in control. In the initial version, it was hard to make smalled changes without overshooting the target.

# Input devices #
- Controller
  * Movement: Joystick or D-pad
  * Jumping: A-button
- Keyboard
  * Movement: WASD or arrow keys
  * Jumping: Space, W or Up arrow
- Touch is the least tested one, and currently only used for being able to show the game easily on the phone. The screen is divided into three areas.
  * Left area: move left
  * Right area: move right
  * Middle area: jump

# Final #
I hope it was possible to follow along. I had to re-write it a couple of times in trying to make it short and concrete. Until next time, here are some early prototype-controls:

<figure>
  <img src="{{ site.baseurl }}/assets/GameDevelopmentPosts/2_Controls/DounbleJumpShooting.gif"/>
  <figcaption>Protagonist double jumping and shooting enemies.</figcaption>
</figure>