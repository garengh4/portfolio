










<svelte:head>
  <title>Home</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>



























<div id="image" />

<!-- <body>
	<div class="center" id="navbar-background">
		<div id="navbar">
			<ul>
				<li><a href="/">Home</a></li>
				<li><a href="/about">About</a></li>
				<li><a href="#">Projects</a></li>
				<li><a href="#">Credits</a></li>
			</ul>
		</div>
	</div>
</body> -->



<!-- ========================================================================================================================================= -->
<style>
	@import url('http://fonts.cdnfonts.com/css/valorant');
	#image {
		background-image: url('/src/images/background.jpg');
	}
	#navbar-background {
		background-color: #0f1923;
		display: block;
		border-radius: 1em;
		padding: 1em 0 0.25em 0;
		width: 50%;
	}

	#navbar {
		text-align: center;
	}

	#navbar li {
		list-style: none;
		display: inline-block;
	}

	#navbar li a {
		margin: 0;
		padding: 9px 18px 9px;
		color: #fff;
		font: normal 12px arial;
		font-size: 35px;
		font-family: 'VALORANT', sans-serif;
	}
	.center {
		margin: auto;
		width: 60%;
		border: 3px solid #73ad21;
		padding: 10px;
	}
</style>
