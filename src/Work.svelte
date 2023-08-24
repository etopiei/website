<script>
    export let logoPath;
    export let name;
    export let title;
    export let timeString;
    export let technolgies;
</script>

<img src={logoPath} alt={name} />
<h4 class="no-indent">{name}</h4>
<br />
<li>{title} - {timeString}</li>
<li>{technolgies}</li>
<div class="job-break" />

<style>
	.job-break {
		margin-top: 16px;
		margin-bottom: 16px;
	}
	img {
		float: left;
		margin-right: 16px;
		width: 100px;
	}
	li {
		list-style: none;
	}
</style>