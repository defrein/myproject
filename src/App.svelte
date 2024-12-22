<script>
	let people = [
		
	];
</script>

<main>
	<h1>People</h1>
	{#each people as person}
		<div>
			<h2>{person.name}</h2>
			<p>is {person.age} years old</p>
			<p>and has a {person.belt} belt</p>
		</div>
	{:else}
		<p>There are no people</p>
	{/each}
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
