<div class="container">
	<nav-content>NavBar</nav-content>
	<main-content>
		<h1>About me</h1>
		<p>
			I am a Software developer, with a focusing interest architecture and cyber-security.
			<br /><br />
			My best web-apps are written with Java, MySQL and Typescript, making the most of the Springboot
			framework following Object Oriented principles in the Model-View-Controller architecture.
		</p>
	</main-content>
	<div id="sidebar">Sidebar: Github Linkedin</div>
	<div id="content-1">Springboot Angular Project</div>
	<div id="content-2">Sveltekit Project</div>
	<div id="content-3">Project 3</div>
	<footer-content>Footer</footer-content>
</div>

<style>
	.container {
		display: grid;
		height: 100vh;
		grid-template-columns: 1fr 1fr 1fr 1fr;
		grid-template-rows: 0.2fr 1.5fr 1.2fr 0.8fr;
		grid-template-areas:
			'nav nav nav nav'
			'sidebar main main main'
			'sidebar content-1 content-2 content-3'
			'sidebar footer footer footer';
		gap: 0.4rem;
		font-family: var(--font-body);
		font-weight: 800;
		font-size: 20px;
		color: var(--font-color)
	}

	nav-content {
		background: #a7ffeb;
		grid-area: nav;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	main-content {
		background: #1d2c4b;
		grid-area: main;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	#sidebar {
		background: #393f48;
		grid-area: sidebar;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	#content-1 {
		background: lightcoral;
		grid-area: content-1;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	#content-2 {
		background: lightgray;
		grid-area: content-2;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	#content-3 {
		background: lemonchiffon;
		grid-area: content-3;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	footer-content {
		background: peru;
		grid-area: footer;
		border-radius: var(--main-radius);
		padding-top: var(--main-padding);
	}

	@media only screen and (max-width: 550px) {
		.container {
			grid-template-columns: 1fr;
			grid-template-rows: 0.4fr 0.4fr 2.2fr 1.2fr 1.2f 1.2fr 1fr;
			grid-template-areas:
				'nav'
				'sidebar'
				'main'
				'content-1'
				'content-2'
				'content-3'
				'footer';
		}
	}
</style>
