<script lang="ts">
	export let text: string;
	export let primary: boolean = true;

	const buttonClass: string = `button-${primary ? 'primary' : 'secondary'}  hard-shadow`;
</script>

<button class={buttonClass} on:click>
	<h4 class="display m-0 tx-shadow">{text}</h4>
</button>

<style lang="scss">
	@use 'sass:map';
	@import 'src/sass/vars.scss';

	.button-primary {
		color: map.get($theme-colors, 'secondary');
		text-align: center;

		background-color: map.get($theme-colors, 'primary');

		border: none;
		border-radius: 2rem 0.25rem;
		padding: 0.75rem 1rem;

		box-shadow: 2px 2px 0px rgba(0, 0, 0, 0.25);

		&:hover {
			background-color: #ff4c14;
		}

		&:active {
			background-color: #ff3c00;
			box-shadow: inset 2px 2px 0px rgba(0, 0, 0, 0.25);
		}
	}

	.button-secondary {
		color: map.get($theme-colors, 'darker');
		text-align: center;

		background-color: map.get($theme-colors, 'lighter');

		border: none;
		border-radius: 2rem 0.25rem;
		padding: 0.75rem 1rem;

		box-shadow: 2px 2px 0px rgba(0, 0, 0, 0.25);

		&:hover {
			background-color: #b0e1bd;
		}

		&:active {
			background-color: #bdffcf;
			box-shadow: inset 2px 2px 0px rgba(0, 0, 0, 0.25);
		}
	}
</style>
