<script lang="ts">
	let clazz: string = '';
	export { clazz as class };

	const cardClass = `ec-card ${clazz}`;
</script>

<div class={cardClass}>
	<slot />
</div>

<style lang="scss">
	@import 'src/sass/colors.scss';
	.ec-card {
		border-radius: 0.5rem;
		transition: all 0.2s ease-out;
	}
	.home-card {
		@media (min-width: 992px) {
			margin: 0 60px 2rem 60px;
		}
		@media (max-width: 992px) {
			margin: 0 2rem 2rem 2rem;
		}
		padding: 6rem 2rem;
	}
</style>
