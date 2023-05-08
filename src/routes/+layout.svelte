<script>
	import Navbar from '../components/navbar.svelte';

	import './styles.scss';
	import 'bootstrap/dist/js/bootstrap.bundle.min.js';
</script>

<main>
	<slot />
	<Navbar />
</main>
