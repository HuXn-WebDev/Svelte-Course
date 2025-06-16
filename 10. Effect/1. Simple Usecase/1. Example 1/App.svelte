<script>
let count = $state(0)

// Here we're logging the count value outside of the $effect, so it will only give us the value once and not when we update the count.
// console.log('------- Count: ', count)

$effect(() => {
    // This effect will run whenever `count` changes.
    console.log('------- Count: ', count)
})
</script>

<section>
    <h1>Count: {count}</h1>
    <button onclick={() => count++}>+</button>
</section>
