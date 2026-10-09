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
	<h3> Home <a href="/projects">Projects</a> <a href="certifications">Certifications</a> <a href="background">Background</a> </h3>
</header>
{@render children()}

<style>
	header{
		font-family: system-ui
	}
	body {
		text-align: left;
	}
</style>