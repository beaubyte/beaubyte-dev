<script lang="ts">
	import favicon from '../../static/favicon.svg';
	import { onNavigate } from '$app/navigation';
	import type { LayoutProps } from './$types';
	let { children }: LayoutProps = $props();
	import { resolve } from '$app/paths';

	onNavigate((navigation) => {
		if (!document.startViewTransition) return; // bailout if browser doesn't support viewTransition

		return new Promise<void>((resolve) => {
			document.startViewTransition(async () => {
				resolve();
				await navigation.complete;
			});
		});
	});
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>BeauByte</title>

</svelte:head>
<header>
	<div id="header-text">
		<h1>// BeauByte</h1>
		<h3> <a href={resolve('/')}>Home</a> <a href="{resolve('/projects')}">Projects</a> <a href={resolve('/certifications')}>Certifications</a> <a href={resolve('/background')}>Background</a></h3>
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
		min-width: 300px;
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
		box-shadow: 0 0 8px 4px;
	}
	header{
		min-width: 300px;
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
	:global(a) {
		color: saddlebrown;
	}
	:global(a:hover) {
			color: chocolate;
	}
	:global(.attached-note) {
		overflow: hidden;
		margin: 20px;
		box-shadow: 0 0 2px 1px;
		background: rgb(255 255 255 / 0.90);
	}
	:global(.attached-note img) {
		position: relative;
		object-fit: scale-down;
		bottom: 20px;
		height: inherit;
		width: inherit;
	}
	:global(.attached-note .staple1){
		position: relative;
		border-bottom-style: ridge;
		border-radius: 5px;
		border-bottom-width: 5px;
		width: 30px;
		rotate:  140deg;
		color: #646464;
		bottom: -5%;
		left: 1%;
	}
	:global(.attached-note .staple2){
		position: relative;
		border-bottom-style: ridge;
		border-radius: 5px;
		border-bottom-width: 5px;
		width: 30px;
		rotate: 220deg;
		color: #646464;
		left: 95%;
		bottom: -5%;
	}
	:global(.attached-note .staple3){
		position: relative;
		border-bottom-style: ridge;
		border-radius: 5px;
		border-bottom-width: 5px;
		width: 30px;
		rotate: 40deg;
		color: #646464;
		bottom: -90%;
		left: 1%;
	}
	:global(.attached-note .staple4){
		position: relative;
		border-bottom-style: ridge;
		border-radius: 5px;
		border-bottom-width: 5px;
		width: 30px;
		rotate: -40deg;
		color: #646464;
		bottom: -90%;
		left: 95%;
	}
  @keyframes fade-in {
      from {
          opacity: 0;
      }
  }

  @keyframes fade-out {
      to {
          opacity: 0;
      }
  }

  :root::view-transition-old(root) {
      animation:
              50ms cubic-bezier(0.4, 0, 1, 1) both fade-out
  }

  :root::view-transition-new(root) {
      animation:
              250ms cubic-bezier(0, 0, 0.2, 1) 90ms both fade-in
  }
  :global(code) {
	  margin: 3px;
  }
</style>