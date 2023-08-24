<script>
	import Project from "./Project.svelte";
    import Work from "./Work.svelte";
	import { projectData } from "./project_data";
	import { workData } from "./work_data";

	export let name;

</script>

<main>
	<h1>{name}</h1>

	<p>My name is really Lachlan Jacob, or as many know me: LJ.</p>
	<p>
		This website is going to be a place for me to showcase some of my
		projects and a little bit about me. Enjoy!
	</p>
	<p>
		To read my thoughts on various topics check out my <a
			href="https://blog.etopiei.com"
			class="no-indent">blog</a
		>. For info on what I've built either myself or with others, read on.
	</p>

	<h3 class="squash">Projects</h3>
	<a href="https://github.com/etopiei">View Code for most of these projects (and more) on GitHub</a>
	<ul class="no-indent">
		<h4 class="no-indent">Completed</h4>
		{#each projectData as project}
			<Project
				name={project.name}
				description={project.description}
				mainLink={project.mainLink}
				extraLinks={project.hasOwnProperty("extraLinks") ? project.extraLinks : null}
			/>
		{/each}
	</ul>

	<h3>Work</h3>
	<p>
		Below is a list of current work I am doing, as well as some of the
		technolgies I use in these jobs.
		<br /> Check out my
		<a
			class="no-indent"
			href="https://www.linkedin.com/in/lachlan-jacob-a14895117/"
			>LinkedIn</a
		> for a more in depth view of my work exerience, education etc.
	</p>
	<ul class="no-indent">
		{#each workData as job}
			<Work
				logoPath={job.logoPath}
				name={job.name}
				title={job.title}
				timeString={job.timeString}
				technolgies={job.technologies}
			/>
		{/each}
	</ul>

	<h3>Experience/Skills</h3>
	<p>
		I enjoy doing HackTheBox and CTFs in my free time, my profiles are shown
		below:
	</p>
	<a href="https://app.hackthebox.eu/profile/76955">HackTheBox Profile</a><br
	/>
	<a href="https://ctftime.org/user/84432">CTF Time Profile</a>
	<p>
		I also am working my way through LeetCode's problems. (<a
			href="https://leetcode.com/etopiei/"
			class="no-indent">Profile Link</a
		>)
	</p>
	<p>
		On the non-technical side I enjoy playing chess (<a
			class="no-indent"
			href="https://lichess.org/@/etopiei">lichess</a
		>,
		<a
			class="no-indent"
			href="https://www.chessmonitor.com/u/ZkQa8N01WyDmxpUSkPpx"
			>chess monitor</a
		>)<br />
		and streaming my speedrunning (<a
			class="no-indent"
			href="https://www.twitch.tv/etopiei">twitch</a
		>,
		<a
			class="no-indent"
			href="https://www.youtube.com/channel/UCrpR5vV2xwLYoIAKF_rpAoQ"
			>youtube</a
		>)<br /><br />
		I also quite enjoy writing music so you can check out my music on:
		<a
			href="https://open.spotify.com/artist/7xEqtE1WYH2QhbQZlOJOjE?si=_4iuyGNmRn6TiTj0b1tOsg"
			class="no-indent">Spotify</a
		>
		or
		<a
			href="https://music.apple.com/us/artist/lachlan-jacob/1530208908"
			class="no-indent">Apple Music</a
		>.
	</p>

	<h3>Contact Me</h3>
	<p>
		I can be reached in a number of ways, my favourites of which are listed
		below:
	</p>
	<ul>
		<li class="no-indent">
			<a href="https://twitter.com/etopiei" class="no-indent">@etopiei</a>
			on twitter
		</li>
		<li class="no-indent">
			email <a href="mailto:me.etopiei@gmail.com" class="no-indent"
				>me.etopiei@gmail.com</a
			>
		</li>
		<br />
		<li class="no-indent">
			or feel free to reach out on <a
				class="no-indent"
				href="https://www.linkedin.com/in/lachlan-jacob-a14895117/"
				>LinkedIn</a
			>
		</li>
	</ul>
</main>

<style>
	* {
		margin-left: 2rem;
		padding-top: 4px;
		padding-bottom: 4px;
	}

	main {
		background-color: #111111e6;
		font-size: 1.4rem;
		color: #b7b7b7;
		margin: 0;
		padding-right: 16px;
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
	li {
		list-style: none;
	}
	h3 {
		color: #874d97;
	}
</style>
