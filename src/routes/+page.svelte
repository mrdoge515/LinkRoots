<script>
	import '../reset.css';
	import Link from '../components/Link.svelte';
	import Title from '../components/Title.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<!-- Icons can be added using path -->
<div>
	<Title title="LinkRoots" />

	<Link name="Discord" url="https://discord.com/" color="#8caaee" />
	<Link name="YouTube" url="https://youtube.com/" color="#e78284" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Github" url="https://github.com/" color="#c6d0f5" />

	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />
	<Link name="Twitch" url="https://twitch.com/" color="#ca9ee6" />

	<Link />

	<Footer />
</div>

<svelte:head>
	<title>mrdoge - LinkRoots</title>
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
