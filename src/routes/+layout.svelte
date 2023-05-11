<script>
	import Navbar from '../components/navbar.svelte';

	import 'bootstrap/dist/css/bootstrap.min.css';
	import '../sass/styles.scss';
</script>

<main>
	<div class="container w-100">
		<slot />
		<Navbar />
	</div>
</main>

<style>
	.container {
		transition: all 0.3s ease-in-out;
	}
</style>
