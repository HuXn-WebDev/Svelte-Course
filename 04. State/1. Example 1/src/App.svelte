<script>
  let count = $state(0);
  let increment = () => count += 1
  let decrement = () => count -= 1
</script>

<h1>Count: {count}</h1>
<button onclick={increment}>+</button>
<button onclick={decrement}>-</button>