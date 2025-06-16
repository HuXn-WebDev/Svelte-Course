<script>
	const products = [
		{
			id: 1,
			name: 'Product 1',
			price: 19.99,
			url: 'https://images.unsplash.com/photo-1426604966848-d7adac402bff?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
		},
		{
			id: 2,
			name: 'Product 2',
			price: 29.99,
			url: 'https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?q=80&w=1948&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
		},
		{ 
			id: 3,
			name: 'Product 3',
		 	price: 39.99,
		 	url: 'https://images.unsplash.com/photo-1541623089466-8e777dd05d70?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
		}
	];
</script>

{#snippet productDisplay(product)}
	<div>
		<img width="200px" src="{product.url}" alt={product.name} />
		<div>
			<h2>{product.name}</h2>
			<span>${product.price.toFixed(2)}</span>
		</div>
	</div>
{/snippet}

{#each products as product}
	{@render productDisplay(product)}
{/each}