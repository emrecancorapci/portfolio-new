<div class="row ec-navbar bg-dark hard-shadow align-items-center">
	<a href="/" class="logo col-12 col-xl-auto col-lg-12 text-center pb-3 pb-xl-0 pb-lg-3">
		<img src="/img/Logo.png" alt="Logo - Emre Can" />
	</a>
	<div class="col" />
	<div
		class="col-12 col-xl-auto col-lg-12 ec-nav bg-lighter hard-shadow d-flex justify-content-center"
	>
		<a href="/" class="tx-shadow-sm">Home</a>
		<a href="/Projects" class="tx-shadow-sm">Projects</a>
		<a href="/About" class="tx-shadow-sm">About</a>
		<a href="/ContactMe" class="tx-shadow-sm">Contact Me</a>
	</div>
</div>

<style lang="scss">
	@use 'sass:map';
	@import 'src/sass/vars.scss';
	@import 'src/sass/colors.scss';

	.logo {
		@media (min-width: 992px) {
			height: 35px;
		}
	}

	.ec-navbar {
		@media (min-width: 992px) {
			margin: 0 8rem;
		}
		@media (max-width: 992px) {
			margin: 0 0rem;
		}
		margin: 0 8rem;
		padding: 1rem 2rem;
		border-radius: 1rem;

		transition: all 0.3s ease-in-out;
	}

	.ec-nav {
		padding: 0.5rem 1rem;
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
