---
layout: post
title:  "Rust - Fibonacci"
date:   2015-12-28 18:28:36
categories: jekyll update
tags:
- rust
- GLSL
---

<img src="{{ site.baseurl }}/assets/portfolio/rustfibonacci/rust-logo.svg" height="200px"/>

I have looked into the relatively new programming language Rust. While doing so I made a graphical application that uses the fibonacci sequence to draw lines. Please see the **[source code][RustFibonacciGit]** for implementation details, but think of the code as quick and dirty since I just wanted to try out the language while doing a fun small project.

I rather like the ideas behind Rust. These quotes from their book describes it pretty well:

> Rust is a systems programming language focused on three goals: safety, speed, and concurrency. It maintains these goals without having a garbage collector... 

> ...Rust improves on current languages targeting this space by having a number of compile-time safety checks that produce no runtime overhead, while eliminating all data races.

The idea of rust seems to be trying to feel lika a high level language like c#, though faster and safer. Rust also has a tool called Cargo which is used for building the code, downloading the dependencies the code needs, and building those dependencies. 

**[Rust 1.0][Rust1]** was released the 15th of May 2015 so it is a relatively new language. This was most noticable when trying to get the open source graphics libraries to work on Windows. I found Glium which worked directly out of the box and was a OpenGL wrapper that did what I needed. Rust has a few open source projects for graphics engines as well.

Visual Code has added Rust to their supported languages and you are also able to run the compiler from within the editor which is nice. See the Visual Code link below for instructions.

####Here are some useful links:####

**[Introduction and book for Rust][RustStart]**

**[Glium - Rust OpenGL wrapper][Glium]**

**[Using Visual Studio Code with Rust][VSStart]**

**[Rust Google Tech Talks][RustGoogleTechTalks]**

**[Rust IDE support][RustIDEs]**

#### Images ####

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
		<li><a href="{{ site.baseurl }}/assets/portfolio/rustfibonacci/fibonacci1.png">
			<img src="{{ site.baseurl }}/assets/portfolio/rustfibonacci/fibonacci1.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/rustfibonacci/fibonacci2.png">
			<img src="{{ site.baseurl }}/assets/portfolio/rustfibonacci/fibonacci2.png"/>
		</a>
		</li>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/rustfibonacci/vs_code.png">
			<img src="{{ site.baseurl }}/assets/portfolio/rustfibonacci/vs_code.png"/>
		</a>
		</li>
	</ul>
</div>

[RustStart]:      http://doc.rust-lang.org/book/README.html
[Glium]:      https://github.com/tomaka/glium
[VSStart]:      https://mobiarch.wordpress.com/2015/06/16/rust-using-visual-studio-code/
[RustGoogleTechTalks]:      https://www.youtube.com/watch?v=d1uraoHM8Gg
[RustIDEs]:      https://www.rust-lang.org/ides.html
[RustFibonacciGit]:      https://github.com/andersnord/rust_fibonacci
[Rust1]:		http://blog.rust-lang.org/2015/05/15/Rust-1.0.html