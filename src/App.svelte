<script>
    // define in main.js
	export let name;
	import Introduction from './Introduction.svelte';
	import Reactivity from './Reactivity.svelte';
	import Props from './Props.svelte';
	import Logic from './Logic.svelte';
	import Lifecycle from './Lifecycle.svelte';

	const pkg = {
	  price: 100,
	  amount: 10
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>

	<Introduction/>
	<Reactivity/>
	<Props answer="hoge" {...pkg}/>
	<Logic/>
	<Lifecycle/>
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