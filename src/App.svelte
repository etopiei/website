<script>
	export let name;
</script>

<style>
	* {
		margin-left: 2rem;
		padding-top: 4px;
		padding-bottom: 4px;
	}

	main {
		background-color:#111111e6;
		font-size: 1.4rem;
		color: #b7b7b7;
		margin: 0;
	}
	h1 {
		color: #874d97;
	}
	p {
		max-width: 800px;
		width: calc(100% - 4rem);
	}
	.no-indent {
		margin-left: 0rem;
	}
	.squash {
		padding: 0;
	}
	footer {
		margin-top: 2rem;
		border-top: solid 1px #e1e1e1;
		border-bottom: solid 1px #e1e1e1;
		padding-top: 8px;
		padding-bottom: 8px;
	}
	li {
		list-style: none;
	}
	h3 {
		color: #874d97;
	}
	img {
		float: left;
		margin-right: 16px;
	}
	.job-break {
		margin-top: 16px;
		margin-bottom: 16px;
	}
</style>

<main>
<h1>{name}</h1>

<p>My name is really Lachlan Jacob, or as many know me: LJ. </p>
<p>This website is going to be a place for me to showcase some of my work, I was going to spend a long time redo-ing this website and fully kitting it out with as many npm modules as I could cram in, but instead I've opted for a more basic approach, which will allow me to focus on working on exciting projects. </p>

<h3 class="squash">Projects</h3>
<a href="https://github.com/etopiei">View Code on GitHub</a>
<ul class="no-indent">
	<h4 class="no-indent">Completed</h4>
	<li><a href="https://github.com/etopiei/QWOP-Bot" class="no-indent">QWOP Bot</a> - A genetic algorithm that learns to play QWOP, powered by websockets and python.</li>
	<li><a href="https://github.com/etopiei/mockapi-cli" class="no-indent">Mockapi CLI</a> - A command line utility to develop mock services quickly </li>
	<li><a href="https://github.com/etopiei/blog" class="no-indent">Blog</a> - The software to run my <a href="https://blog.etopiei.com" class="no-indent">blog.</a></li>
	<li><a href="https://github.com/etopiei/website" class="no-indent">Website</a> - The code for this website</li>
	<li><a href="https://github.com/etopiei/lumino" class="no-indent">Lumino</a> - A hackathon project to make Public Transport trips safer.</li>
	<li><a href="https://github.com/etopiei/DSPM" class="no-indent">DSPM</a> (Dead Simple Password Manager) - A python CLI app to manage and generate passwords.</li>
	<h4 class="no-indent">Coming Soon or WIP</h4>
	<li><a href="https://zappcast.com" class="no-indent">ZappCast</a> - A programming podcast hosted by myself and a few friends.</li>
	<li><a class="no-indent" href="https://github.com/etopiei/kayo/">Kayo App</a> - Desktop app for watching sport with Kayo.</li>
	<li>Open Chess Browser - A chess game explorer built with Rust and Neo4j (Coming Soon) </li>
</ul>

<h3>Work</h3>
<p>Below is a list of current work I am doing,
 as well as some of the technolgies I use in these jobs.
 <br> Check out my <a class="no-indent" href="https://www.linkedin.com/in/lachlan-jacob-a14895117/">LinkedIn</a> for a more in depth view of my work exerience, education etc.</p>
<ul class="no-indent">
	<img src="./nab.png" alt="NAB">
	<h4 class="no-indent">National Australia Bank</h4><br>
		<li> Software Engineer - January 2019 -> Present</li>
		<li>React, Typescript, Express, Java, AWS, Docker</li>
	<div class="job-break"></div>
	<img src="./ai.png" alt="AI Media">
	<h4 class="no-indent">AI Media</h4><br>
		<li>Software Developer - July 2018 -> Present</li>
		<li>PHP, Vue, MYSQL, Python, Linux Admin, AWS, cPanel</li>
</ul>

<h3>Contact Me</h3>
<p>I can be reached in a number of ways, my favourites of which are listed below:</p>
<ul>
	<li class="no-indent"><a href="https://twitter.com/etopiei" class="no-indent">@etopiei</a> on twitter</li>
	<li class="no-indent">email <a href="mailto:etopiei@tech.melbourne" class="no-indent">etopiei@tech.melbourne</a></li>
	<li class="no-indent">email <a href="mailto:me.etopiei@gmail.com" class="no-indent">me.etopiei@gmail.com</a></li><br>
	<li class="no-indent">or feel free to reach out on LinkedIn (linked above)</li>
</ul>


<footer class="no-indent">
<span>© Copyright 2020 - etopiei</span>
</footer>
</main>
