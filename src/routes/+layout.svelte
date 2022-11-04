<!-- Note:+layout.svelte will appear in all routes' +page.svelte -->

<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<!-- ============================================================================================================================ -->

<!-- header -->
<div class="app">
	<Header />

  <!-- app content -->
	<main>
		<slot />
	</main>

  <!-- footer -->
	<footer>
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
	</footer>
</div>

<!-- ============================================================================================================================ -->

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		display: flex;
		flex-direction: column;
		padding: 2rem;
		width: 100%;
		max-width: 100rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
