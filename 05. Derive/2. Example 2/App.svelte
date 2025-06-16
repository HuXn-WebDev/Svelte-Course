<script>
  let price = $state(100);
  let quantity = $state(2);

  let total = $derived(price * quantity);
</script>

<h2>Price: ${price}</h2>
<h2>Quantity: {quantity}</h2>
<h2>Total: ${total}</h2>

<input type="number" bind:value={price} placeholder="Price" />
<input type="number" bind:value={quantity} placeholder="Quantity" />
