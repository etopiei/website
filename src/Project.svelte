<script>
    export let mainLink;
    export let name;
    export let description;
    export let extraLinks = null;
</script>

<li>
    <a href={mainLink} class="no-indent">{name}</a> - {description}
        {#if extraLinks}
        (
            {#each extraLinks as {text, link}, index}
                <a href={link} class="no-indent">{text}</a>
                {index !== extraLinks.length - 1 ? ", " : ""}
            {/each}
        )
        {/if}
</li>

<style>
	li {
        margin-top: 4px;
        margin-bottom: 4px;
		list-style: none;
	}
	.no-indent {
		margin-left: 0rem;
	}
	* {
		margin-left: 2rem;
		padding-top: 4px;
		padding-bottom: 4px;
	}
</style>