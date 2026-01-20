---
layout: home
title: Home
---

<div id ="intro-wrapper" class="l-middle">
	<div id="intro-title-wrapper" class="intro-left">
		<h1 id="intro-title">Hi, I'm Etash Guha</h1>
		<div id="intro-subtitle">
			I'm a Ph.D. student in the Stanford CS Department.
		</div>
	</div>
	<div class="intro-left">
	<div class="intro-left">
		I research how to design and improve training data curation protocols for training large text and image models. This includes synthetic data generation, data filtering, and online data sampling. I am <b>extremely</b> fortunate  to be advised by the amazing Professors <a href="https://people.csail.mit.edu/ludwigs"> Ludwig Schmidt</a> and <a href="https://homes.cs.washington.edu/~yejin"> Yejin Choi</a>. I'm graciously supported by the NSF Graduate Research Fellowship. 
	</div>
	<div style="height: 1rem"></div>
	<div class="intro-left">
		I was a researcher at <a href="https://sambanova.ai/?gclid=CjwKCAiAqIKNBhAIEiwAu_ZLDr2s7pJ9vwSq0IiztdcXjYXR4VyjhZznyNNJ1QiqNxQw6M7PjVBJqBoCKYsQAvD_BwE">SambaNova Systems</a> working on the reliability of Large Language Models. Most recently, I was a research intern under <a href="https://emtiyaz.github.io/">Dr. Emtiyaz Khan</a> on the Approximate Bayesian Inference Team at RIKEN AIP in Tokyo, Japan. I was both an undergraduate student and research assistant at Georgia Tech where I worked with <a href="https://vmuthukumar.ece.gatech.edu/">Vidya Muthukumar</a>, <a href="https://sites.gatech.edu/ashwin-pananjady">Ashwin Pananjady</a>,  <a href="https://faculty.cc.gatech.edu/~jabernethy9"> Jacob Abernethy</a>, and <a href="https://www.isye.gatech.edu/users/xiaoming-huo">Xiaoming Huo</a>. 
	</div>
	<div style="height: 1rem"></div>
	<div>
		I have worked with researchers, traders, and software engineers while working at <a href="https://www.bespokelabs.ai/">Bespoke Labs</a>, <a href="https://sambanova.ai/?gclid=CjwKCAiAqIKNBhAIEiwAu_ZLDr2s7pJ9vwSq0IiztdcXjYXR4VyjhZznyNNJ1QiqNxQw6M7PjVBJqBoCKYsQAvD_BwE">SambaNova Systems</a>, <a href="https://www.fortlp.com/">FORT LP</a>, and <a href="https://www.sas.com/en_us/home.html">SAS</a>.
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
		<div id="intro-cv"><a href="/cv">Here's my CV.</a></div>
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


