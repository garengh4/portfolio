<div class="container">
	<nav>NavBar</nav>
	<main>About me: resume</main>
	<div id="sidebar">Sidebar: Github Linkedin</div>
	<div id="content-1">Project 1</div>
	<div id="content-2">Project 2</div>
	<div id="content-3">Project 3</div>
	<footer>Footer</footer>
</div>

<style>
  :root{
    --main-radius:5px;
    --main-padding: 10px;
  }
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
    font-family: 'Times New Roman', Times, serif;
    font-weight: 800;
    font-size: 20px;
    color: #EAEFB4;

	}
	nav {
		background: #a7ffeb;
		grid-area: nav;
    border-radius: var(--main-radius);
    padding-top: var(--main-padding);
	}
	main {
		background: #1D2C4B;
		grid-area: main;
    border-radius: var(--main-radius);
    padding-top: var(--main-padding);
	}
	#sidebar {
		background: #393F48;
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
	footer {
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
