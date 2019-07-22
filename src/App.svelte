<script>
	export let name;
</script>

<style>
	* {
		margin-left: 2rem;
		padding-top: 4px;
		padding-bottom: 4px;
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
</style>

<h1>{name}</h1>

<p>My name is really Lachlan Jacob, or as many know me: LJ. </p>
<p>This website is going to be a place for me to showcase some of my work, I was going to spend a long time redo-ing this website and fully kitting it out with as many npm modules as I could cram in, but instead I've opted for a more basic approach, which will allow me to focus on working on exciting projects. </p>
<p>I've picked Svelte for my website because I really like the way it feels and it's simplicity. Stay tuned for more content coming soon.</p>

<h3 class="squash">Projects</h3>
<ul class="no-indent">
	<h4 class="no-indent">Coming Soon or WIP</h4>
	<li><a class="no-indent" href="https://github.com/etopiei/kayo/">Kayo App</a> - Desktop app for watching sport with Kayo.</li>
	<li>Open Chess Browser - A chess game explorer built with Rust and Neo4j (Coming Soon) </li>
	<h4 class="no-indent">Completed</h4>
	<li><a href="https://github.com/etopiei/mockapi-cli" class="no-indent">Mockapi CLI</a> - A command line utility to develop mock services quickly </li>
	<li><a href="https://github.com/etopiei/blog" class="no-indent">Blog</a> - The software to run my blog.</li>
</ul>

<h3>Work</h3>
<ul class="no-indent">
	<h4 class="no-indent">National Australia Bank</h4>
		<li> Intern Software Engineer - January 2019 -> Present</li>
		<li>React, Typescript, Express, Java, AWS, Docker</li>
	<h4 class="no-indent">AI Media</h4>
		<li>Software Developer - July 2018 -> Present</li>
		<li>PHP, Vue, MYSQL, Python, Linux Admin, AWS, cPanel</li>
</ul>

<h3>Education</h3>
<ul class="no-indent">
	<h4 class="no-indent">Monash University</h4>
	<li>Bachelor of Computer Science - 2017 -> Present</li>
</ul>

<footer class="no-indent">
<span>© Copyright 2019 - etopiei</span>
</footer>
