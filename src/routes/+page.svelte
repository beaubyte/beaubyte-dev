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
		background: saddlebrown;
		padding: 14px;
		border-radius: 5px;
		margin: 2px;
		color: white;
	}
	details p {
		cursor: text;
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
		<details name="positions">
			<summary>Cybersecurity Analyst</summary>
			<p>
				UW-Stout Polytechnic ranks as a top Cybersecurity school in the United States. We learn intrusion detection, building
				resilient and secure networks, and finding, exploiting, and defending against different threat vectors.
				I have experience working with metasploit, hashcat, nmap, and many other tools in simulated networks to
				find attacks and privilege escalations. My project <code>bt-le-investigator</code> was built to show a
				potential malicious use of Bluetooth MAC addresses, and I build different devices and scripts to use on the field
				when demonstrating vulnerabilities.
			</p>
		</details>
		<details name="positions">
			<summary>Network Engineer</summary>
			<p>
				I have a CCNA, and have worked extensively with Cisco equipment in configuration and automation. At my
				internship with Kwik Trip, I worked with cloud-managed Meraki switches, Catalyst Center, and SD-WAN Manager.
				I also worked with cloud-based Mist APs, and Ansible for configuration and automation. I am very adaptable,
				and can understand and ramp up quickly to your environment.
			</p>
		</details>
		<details name="positions">
			<summary>Systems Administrator</summary>
			<p>
				I have a homelab that I run for my own personal services and applications. I am knowledgeable with
				container platforms like Docker and Proxmox, and general Linux server administration and best security
				practices. I have experience routing services through reverse proxies, Tailscale services, and creating
				service-specific firewall rules for services when needed. I work declaratively when possible, with docker
				compose files and git for Tailscale routing rules, Ansible automations, and pretty much anything that goes
				through iterative development.
			</p>
		</details>
		<details name="positions">
			<summary>Software Developer</summary>
			<p>
				I develop my own applications and services to improve various things in my life. I have done Python automation
				work at my jobs at UW-Stout Polytechnic and Kwik Trip, using git for version control. I have experience
				working in Agile, and with building GitHub Actions for code linting, tests, and deployment. I hand-build all
				applications that I make, and seek to have strong understandings of the libraries that I work with. I am
				strongest in C++, but have experience with Java, Python, and web development as well. While I don't use AI
				for writing any of my projects, I have experience with LLMs dating back to pre-GPT3 tools like Inferkit, and
				I utilize Claude's API through AWS Bedrock in my <code>shocarlo-text-formatter</code> project. Vim keybindings
				are my friend.
			</p>
		</details>
		<div>
			<p>
			Get in touch with me at <a href="mailto:contact@beaubyte.dev">contact@beaubyte.dev</a>
			</p>
			</div>
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
