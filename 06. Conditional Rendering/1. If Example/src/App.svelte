<script>
  let isVisible = $state(true);
</script>

{#if isVisible}
  <p>The message is visible!</p>
{/if}

<button onclick={() => isVisible = !isVisible}>
  Toggle Message
</button>