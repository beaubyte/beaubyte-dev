<script lang="ts">
	import favicon from '#lib/assets/favicon.svg';
	import type { LayoutProps } from './$types';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>BeauByte</title>

</svelte:head>
<header>
	<h1>// BeauByte</h1>
	<h3 style="padding-left: 10px"> <a href="/">Home</a> <a href="/projects">Projects</a> <a href="certifications">Certifications</a> <a href="background">Background</a></h3>
</header>
{@render children()}

<style>
	@import url('https://fonts.googleapis.com/css2?family=Literata:ital,opsz,wght@0,7..72,200..900;1,7..72,200..900&display=swap');
	:global(body) {
		text-align: left;
		max-width: 800px;
		min-width: 400px;
		background-color: #fbf8f2;
		margin: 0 auto;
		padding-left: 25px;
		padding-right: 25px;
		border-left-style: dotted;
		border-right-style: dotted;

	}
	header{
		font-family: Literata, serif;
		min-width: 400px;
		max-width: 800px;
		word-spacing: 8px;
		margin-top: 20px;
		padding-left: 10px;
		padding-right: 10px;
		border-style: double;
	}



</style>