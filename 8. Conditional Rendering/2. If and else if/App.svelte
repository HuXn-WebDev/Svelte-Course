<script>
	let score = $state(80);
</script>

{#if score >= 90}
	<p>Excellent</p>
{:else if score >= 75}
	<p>Good</p>
{/if}

<p>Score: {score}</p>
<button onclick={() => score += 5}>Increase Score</button>
<button onclick={() => score -= 5}>Decrease Score</button>