<script>
	let src = 'https://svelte.dev/tutorial/image.gif';
	let name = 'Rick Astley';
    let string = `this string contains some <strong>HTML!!!</strong>`;
</script>

<p>This is sample component.</p>
<img {src} alt="{name} dances.">
<p>{@html string}</p>

<style>
	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>
