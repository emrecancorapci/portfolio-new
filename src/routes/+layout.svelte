<script>
	import Navbar from '../components/navbar.svelte';

    import '../sass/styles.scss'
</script>

<main>
	<div class="container">
		<slot />
		<Navbar />
	</div>
</main>

<style lang="scss">
	main {
        display: flex;
        justify-content: center;
        align-items: center;

		font-family: 'Space Grotesk', sans-serif;
		font-style: normal;
		background-color: #cece86;
		height: 100vh;
		width: 100vw;
	}
</style>
