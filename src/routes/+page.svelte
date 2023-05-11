<script>
	import Button from '../components/button.svelte';
	import Card from '../components/card.svelte';
</script>

<svelte:head>
	<title>Emre Can Çorapçı Portfolio</title>
</svelte:head>

<Card class="row home-card bg-dark hard-shadow-lg">
	<div class="col">
		<div class="row mb-2 gap-3 mb-3">
			<Card class="col-12 col-xl-5 col-lg-12 tx-darker bg-lighter hard-shadow-lg p-4 text-end">
				<h4 class="tx-shadow-sm">software developer</h4>
				<h1 class="display tx-shadow-sm">Emre Can Çorapçı</h1>
				<h3 class="tx-shadow-sm">
					emre can is not a world-renowned software developer, but he tries to do his job well.
				</h3>
			</Card>
			<Card class="col bg-primary hard-shadow-lg">COL-7</Card>
		</div>
		<div class="row mt-2 gap-3">
			<Card class="col bg-primary hard-shadow-lg">COL-4</Card>
			<Card class="col-3  bg-darker hard-shadow-lg py-2 px-3 gap-2">
				<h2 class="display tx-shadow-sm w-100 text-end tx-lighter">
					I'm currently working as Managing Partner and Front-End Developer at an enterprise called
				</h2>
				<h1 class="display tx-white w-100 text-end tx-shadow">Eneftimbu</h1>
			</Card>
			<div class="col-5 p-3">
				<div class="row">
					<div class="col-6">
						<h1 class="tx-commit-num tx-white tx-shadow-lg">350+</h1>
					</div>
					<div class="col-3">
						<div class="row align-items-center h-100 ms-3">
							<h3 class="col-12 tx-lighter display tx-shadow">Public Commits</h3>
						</div>
					</div>
				</div>
				<div class="row justify-content-center">
					<div class="col-3">
						<h1 class="tx-commit-num tx-white tx-shadow-lg">26</h1>
					</div>
					<div class="col-3">
						<div class="row align-items-center h-100 ms-3">
							<h3 class="col-12 tx-lighter display tx-shadow">Public Commits</h3>
						</div>
					</div>
				</div>
				<div class="row">
					<div class="col-12">
						<h2 class="tx-secondary text-center tx-shadow">
							written in C#, C++, JavaScript and more...
						</h2>
					</div>
				</div>
				<a class="row pt-2" href="/Projects">
					<Button text="View Projects" />
				</a>
			</div>
		</div>
	</div>
</Card>

<style lang="scss">
	@import 'src/sass/colors.scss';

	.tx-commit-num {
		font-size: 96px;
		line-height: 75%;
	}
</style>
