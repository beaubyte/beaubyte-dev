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
	<div id="header-text">
		<h1>// BeauByte</h1>
		<h3> <a href="/">Home</a> <a href="/projects">Projects</a> <a href="certifications">Certifications</a> <a href="background">Background</a></h3>
	</div>
</header>
{@render children()}

<style>
	@import url('https://fonts.googleapis.com/css2?family=Literata:ital,opsz,wght@0,7..72,200..900;1,7..72,200..900&display=swap');
	:global(html) {
		background-color: #fff6ee;
	}
	:global(body) {
		text-align: left;
		max-width: 800px;
		min-width: 400px;
		background-color: #fbf8f2;
		margin: 0 auto;
		padding-left: 25px;
		padding-right: 25px;
		border-left-style: dotted;
		border-left-width: 8px;
		border-right-width: 8px;
		border-right-style: dotted;
		font-family: Literata, serif;
		padding-bottom: 50px;
		box-shadow: 0px 0px 8px 4px;
	}
	header{
		min-width: 400px;
		max-width: 800px;
		word-spacing: 8px;
		padding-top: 20px;

	}
	#header-text{
		padding-left: 20px;
		padding-right: 20px;
		border-style: double;
		border-width: 8px;
	}

	:global(hr) {
			background-color: black;
			height: 1px;
			margin: 2px;
	}

	:global(.darken){
			filter: brightness(0);
	}
	a {
			color: #000000;
	}
	a:hover {
			color: chocolate;
	}


</style>