<div class="row navbar hard-shadow">
	<div class="col-auto">
		<a href="/">
			<img src="/img/Logo.png" alt="Logo - Emre Can">
        </a>
	</div>
	<div class="col" />
	<div class="col-auto nav hard-shadow">
		<a href="/" class="text-shadow-sm">Home</a>
		<a href="/Projects" class="text-shadow-sm">Projects</a>
		<a href="/About" class="text-shadow-sm">About</a>
		<a href="/ContactMe" class="text-shadow-sm">Contact Me</a>
	</div>
</div>

<style lang="scss">
	@use 'sass:map';
	@import 'src/sass/styles.scss';

	.navbar {
        margin: 0 8rem;
		padding: 1rem 2rem;
		background-color: map.get($theme-colors, 'dark');
		border-radius: 1rem;
	}

	.nav {
		padding: 0.5rem 1rem;
		background-color: map.get($theme-colors, 'lighter');
		border-radius: 32px 4px;

		a {
			padding: 0 1rem;
			color: map.get($theme-colors, 'darker');

            &:hover {
                color: map.get($theme-colors, 'white');
            }

            &:active {
                color: map.get($theme-colors, 'secondary');
            }

            .active {
                color: map.get($theme-colors, 'primary');
            }
		}
	}
</style>
