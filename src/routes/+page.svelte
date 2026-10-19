<script>
	import uwstoutlogo from '#lib/assets/uwstout.svg';
</script>

<style>
	#homebox {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-items: flex-start;
		justify-content: space-between;
	}
	ul {
		padding-left: 0;
	}
	li {
		margin: 5px;
	}
	details {
		cursor: pointer;
	}
</style>

<div id="homebox">
	<div style="max-width: 450px; min-width: 300px;">
		<h3>Welcome!</h3>
		<p>I am a 20-year old cybersecurity student based out of Western Wisconsin.</p>
		<p>I study Cybersecurity at the University of Wisconsin-Stout Polytechnic. I am pursuing a <i>B.S. in Cybersecurity</i>,
		with minors in <i>Information Security Management</i>, <i>Network Systems & Design</i>, and <i>Computer Science</i>.</p>
		<p>Currently seeking full-time work in the Eau Claire or Twin Cities metro areas.</p>
		<h4>How I could serve well as a:</h4>
		<details>
			<summary>Cybersecurity Analyst</summary>
		</details>
		<details>
			<summary>Network <svg height=0>
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
Engineer</summary>
		</details>
		<details>
			<summary>Systems Administrator</summary>
		</details>
		<details>
			<summary>Software Developer</summary>
		</details>
	</div>
	<div style="max-width: 250px;">
		<img src={uwstoutlogo} height="50px;" alt="Logo for UW-Stout" class="darken" style="padding-top: 10px; padding-left: 15%">
		<p style="font-size: 10pt; margin: 0"><i>September 2024 - May 2027 (Expected)</i></p>
		<h4>
			Experience with:
		</h4>
		<ul>
			<li>Cisco networking concepts, including standard CCNA and higher-level topics.</li>
			<li>Configuring, interfacing, and using relational (MySQL, PostgreSQL) databases and their applications in software.</li>
			<li>Web Design, including both frontend and backend.</li>
			<li>Cloud Computing with Amazon Web Services, as well as in Azure and Google Cloud.</li>
			<li>GNU/Linux and Windows operating systems, including different desktop and embedded usage applications.</li>
			<li>Comfortable in C++ and Java programming languages, with experience in Python for automation and scripting.</li>
			<li>Cisco SD-WAN Networking, including how to build and maintain an efficient fabric utilizing OMP routing.</li>
		</ul>
	</div>
</div>
