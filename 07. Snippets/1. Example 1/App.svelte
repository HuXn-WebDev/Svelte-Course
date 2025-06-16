<script>
	const users = [
		{ id: 1, name: 'Alice', age: 28, location: 'New York' },
		{ id: 2, name: 'Bob', age: 34, location: 'London' },
		{ id: 3, name: 'Charlie', age: 25, location: 'Berlin' }
	];
</script>


{#snippet userCard(user)}
	<section>
		<h3>Name: {user.name}</h3>
		<p>Age: {user.age}</p>
		<p>Location: {user.location}</p>
	</section>
{/snippet}

{#each users as user}
	{@render userCard(user)}
{/each}

