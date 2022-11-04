hello from fallback +page.svelte
<div class="text-column">
  hello from text-column
</div>
<div class="grid-container ">
	<div class="left-console">LEFT</div>
  <h1>hello h1</h1>
  <a href="#">hello a</a>
  <p>hello p</p>
</div>
TODO: FIX

<style>
	.grid-container {
		display: grid;
		width: 100%;
		height: 250px;
		grid-template-areas:
			'head head'
			'nav  main'
			'nav  foot';
		grid-template-rows: 50px 1fr 30px;
		grid-template-columns: 150px 1fr;
	}
	.grid-container > div {
		grid-area: nav;
		background-color: #ffa08c;
	}
</style>
