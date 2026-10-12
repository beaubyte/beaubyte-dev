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
<svg height=0>
	<filter id="feblend">
		<feTurbulence baseFrequency="0.8" numOctaves="6" result="turb" seed="200"/>
		<feDisplacementMap in="SourceGraphic" in2="turb" scale="20" xChannelSelector="B" yChannelSelector="A"/>
		<feComposite operator="out" in="SourceGraphic" in2="offset-turb" result="inverse"/>
		<feFlood flood-color="black" flood-opacity="0.05" result="color"/>
		<feComposite operator="atop" in="color" in2="inverse" result="shadow"/>
		<feBlend in="shadow" in2="SourceGraphic" mode="multiply"/>
	</filter>
	<!-- credit to @alexmwalker for the filter -->
</svg>
{@render children()}

<style>
	@import url('https://fonts.googleapis.com/css2?family=Literata:ital,opsz,wght@0,7..72,200..900;1,7..72,200..900&display=swap');
	:global(html) {
		background-color: #fff6ee;
	}
	:global(body) {
		filter: url("#feblend");
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


</style>