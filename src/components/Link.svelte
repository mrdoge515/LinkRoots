<script>
	import FaDiscord from 'svelte-icons/fa/FaDiscord.svelte';
	import FaYoutube from 'svelte-icons/fa/FaYoutube.svelte';
	import FaTwitch from 'svelte-icons/fa/FaTwitch.svelte';
	import FaGithub from 'svelte-icons/fa/FaGithub.svelte';

	export let name = 'undefined';
	export let url = 'undefined';
	export let color = 'red';
</script>

<a target="_blank" rel="noreferrer" href={url} style="--border-color: {color}">
	<div class="icon">
		{#if name === 'Discord'}
			<div class="icon"><FaDiscord /></div>
		{:else if name === 'YouTube'}
			<div class="icon"><FaYoutube /></div>
		{:else if name === 'Twitch'}
			<div class="icon"><FaTwitch /></div>
		{:else if name === 'Github'}
			<div class="icon"><FaGithub /></div>
		{/if}
	</div>

	{#if name === 'undefined' || url === 'undefined' || color === 'red'}
		<span class="undefined">{name}</span>
	{:else}
		<span>{name}</span>
	{/if}
</a>

<style>
	a {
		width: 60%;
		padding: 1em;
		margin: 0.5em;

		border: solid 0.3em var(--border-color);
		border-radius: 2em;

		color: #b5bfe2;
		background-color: #292c3c;
		font-size: 1.5em;
		text-align: center;
		font-family: 'Roboto', sans-serif;
		text-decoration: none;

		transition-property: color background-color;
		transition: ease-in 0.3s;

		text-shadow: -4px 3px black;
	}
	a:hover {
		color: var(--border-color);
		background-color: #232634;
	}
	.icon {
		height: 2em;
		display: inline-block;
		vertical-align: middle;
		filter: drop-shadow(-2px 2px black);
		margin-right: 0.1em;
	}
	.undefined {
		animation: undefined 3s infinite;
	}

	@keyframes undefined {
		0% {
			color: #ea999c;
			border-color: #8caaee;
		}
		50% {
			color: #8caaee;
			border-color: #ea999c;
		}
		100% {
			color: #ea999c;
			border-color: #8caaee;
		}
	}

	@media only screen and (min-width: 1000px) {
		a {
			width: 20%;
			padding: 1.5em 2em;
			margin: 0.8em;
			font-size: 2em;
		}
	}
</style>
