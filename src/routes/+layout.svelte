<script lang="ts">
	import favicon from '#lib/assets/favicon.svg';
	import type { LayoutProps } from './$types';

	let { children }: LayoutProps = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<h1>BeauByte</h1>
	<h3> Home Projects Certifications Background</h3>
</svelte:head>

{@render children()}
