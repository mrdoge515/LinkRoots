<script>
	import '../reset.css';
	import Link from '../components/Link.svelte';
	import Title from '../components/Title.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<div>
	<Title title="mrdoge's links" />

	<Link name="YouTube" url="https://www.youtube.com/@mrdoge515" color="#e78284" />
	<Link name="Twitch" url="https://www.twitch.tv/mrdoge___" color="#ca9ee6" />
	<Link name="Github" url="https://github.com/mrdoge515/" color="#c6d0f5" />

	<Footer />
</div>

<svelte:head>
	<title>LinkRoots</title>
</svelte:head>

<style>
	div {
		min-height: 100%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex-shrink: inherit;
		background-color: #303446;
	}
</style>
