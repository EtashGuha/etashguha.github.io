---
layout: home
title: Home
---

<div id ="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper" class="intro-left">
		<h1 id="intro-title">Hi, I'm Etash Guha</h1>
		<div id="intro-subtitle">
			I'm an undergraduate CS student at Georgia Tech. 
		</div>
	</div>
	<div class="intro-left">
	<div class="intro-left">
		I research how to use <b>Machine Learning Theory</b> to solve Combinatorial Optimization problems. Specifically, I utilize ideas from  <b>Online Learning and Mean Field Theory</b> in order to create algorithms that generate approximate solutions to difficult NP-Hard problems efficiently and accurately. I also work on the applications of using Combinatorial Optimization within Systems for ML. 
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I am currently a Senior at Georgia Tech studying CS with threads in Intelligence and Theory. I was previously advised by <a href="https://www.linkedin.com/in/le-song-03223813">Le Song</a> in the Machine Learning Lab. I am now currently advised by <a href="https://vmuthukumar.ece.gatech.edu/">Vidya Muthukumar</a> and <a href="https://sites.gatech.edu/ashwin-pananjady">Ashwin Pananjady.</a>
	</div>
	<div style="height: 1rem"></div>
	<div>
		I have worked with researchers, traders, and software engineers while working at <a href="https://sambanova.ai/?gclid=CjwKCAiAqIKNBhAIEiwAu_ZLDr2s7pJ9vwSq0IiztdcXjYXR4VyjhZznyNNJ1QiqNxQw6M7PjVBJqBoCKYsQAvD_BwE">SambaNova Systems</a>, <a href="https://www.fortlp.com/">FORT LP</a>, and <a href="https://www.sas.com/en_us/home.html">SAS</a>.
	</div>
	<!-- <div style="height: 1rem"></div>
	<div>
		My research is supported by a <a href="https://www.nasa.gov/strg/nstrf">NASA Space Technology Research Fellowship</a>.
	</div> -->
</div>

<div class="intro-right">
	<img id="intro-image" class="intro-right" src="/images/portrait.jpg">
	<div style="height: 0.5rem"></div>
	<div id="intro-image-links" class="intro-right">
		{% for link in site.data.social-links %}
			{% if link.on-homepage == true %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	<div style="height: 0.5rem"></div>
	<div id="intro-cv-wrapper" class="intro-right">
		{% for link in site.data.social-links %}
			{% if link.id == "cv-web" %}
				{% include social-link.html link=link %}
			{% endif %}
		{% endfor %}
		<!-- <div id="intro-cv"><a href="/cv">Here's my CV.</a></div> -->
	</div>
	</div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title l-middle">
	Featured <a href="/cv#publications">Research Publications</a>
</h2>
<div class="cover-wrapper l-screen">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>


<!-- <p class="l-middle intro-text" markdown="1">
	Including a list of [projects][projects], the [blog][blog], [monthly music playlists][monthly-music], [stuff I use][stuff-i-use], and the [archive][archive].
</p> -->



[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"