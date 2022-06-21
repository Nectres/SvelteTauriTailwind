<script lang="ts">
	export let name: string;
	let count: number = 0;
</script>

<main>
	<div class="bg-black text-white">Good morning, {name}</div>
	<h1 class="text-red-900">Hello {name}!</h1>
	<p>You have clicked the button: {count} time(s)</p>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	<button on:click={_ => count += 1}>Click</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>