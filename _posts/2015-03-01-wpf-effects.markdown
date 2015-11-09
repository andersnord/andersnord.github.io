---
layout: post
title:  "WPF Effects"
date:   2015-03-01 18:28:36
categories: jekyll update
avatarurl: /assets/about/profile.png
tags:
- WPF
- C#
---

<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/all4.png" height="200px"/> 

In this post I will be talking shortly about using pixel shaders written in HLSL for WPF. These can be used to create more advanced visual effects. In my example I have created some procedural noise shaders, such as perlin noise and voronoi noise 2D and 3D. Notice that they will animate when clicked. **[Source code here][GitHubLink]**.

WPF has a base class called ShaderEffect that is used by all effects. By using this class it is possible to wrap HLSL pixel shaders and apply them to elements in XAML. Dependency properties are bound to the HLSL input like this:

**C-Sharp:**

{% highlight csharp %}
public class SimplexNoise : ShaderEffect
{
	public static readonly DependencyProperty SizeProperty = DependencyProperty.Register("Size", typeof(double), typeof(SimplexNoise), new UIPropertyMetadata(((double)(10D)), PixelShaderConstantCallback(0)));

	public SimplexNoise()
	{
	    ...
	    
	    this.UpdateShaderValue(SizeProperty);
	}

	public double Size
	{
	    get { return ((double)(this.GetValue(SizeProperty))); }
	    set { this.SetValue(SizeProperty, value); }
	}
}
{% endhighlight %}

**HLSL Shader:**

{% highlight c %}

float size : register(C0);

...

float4 main(float2 uv : TEXCOORD) : COLOR
{
	float perlin = 0.5 + 0.5 * snoise(float3(size * uv, timer * animationspeed));

	...

  	return finalColor;
}
{% endhighlight %}

**XAML:**

{% highlight html %}
<CheckBox.Effect>
    <effects:SimplexNoise 
	    ...
	    Size="{Binding Value, ElementName=SizeInput}"
    />
</CheckBox.Effect>
{% endhighlight %}

There is a lot of code missing here, but I just wanted to show the basic idea. Please look att the **[source code][GitHubLink]** for a more detailed version.

A great tool for helping out is the shader editor **[Shazzam][shazzam]**. Shazzam also compiles the .fx files into .ps files and generates C# wrappers, which is really handy. It supports Shader Model 3 pixel shaders (can be set under Settings). 

For a much more detailed explanation for how to implement pixel shaders in WPF, please visit this **[this Shader Effect tutorial][ShaderEffectTutorial]**.

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
		<li><a href="{{ site.baseurl }}/assets/portfolio/wpfeffect/simplexnoise.png">
			<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/simplexnoise.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/wpfeffect/voronoirings.png">
			<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/voronoirings.png"/>
		</a>
		</li>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/wpfeffect/voronoi3dcellular.png">
			<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/voronoi3dcellular.png"/>
		</a>
		</li>
	</ul>

		<ul id="menu">
		<li><a href="{{ site.baseurl }}/assets/portfolio/wpfeffect/simplexnoise_button.png">
			<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/simplexnoise_button.png"/>
		</a>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/wpfeffect/voronoi2d.png">
			<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/voronoi2d.png"/>
		</a>
		</li>
		</li>
		  	<li><a href="{{ site.baseurl }}/assets/portfolio/wpfeffect/application.png">
			<img src="{{ site.baseurl }}/assets/portfolio/wpfeffect/application.png"/>
		</a>
		</li>
	</ul>
</div>

[GitHubLink]:      https://github.com/andersnord/wpfeffects
[shazzam]:	http://shazzam.software.informer.com/1.4/
[ShaderEffectTutorial]: http://www.codeproject.com/Articles/71617/Getting-Started-with-Shader-Effects-in-WPF
