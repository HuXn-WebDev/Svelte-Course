<script>
	let hour = $state(20); 
</script>

{#if hour < 12}
	<p>Good Morning</p>
{:else if hour < 18}
	<p>Good Afternoon</p>
{:else}
	<p>Good Evening</p>
{/if}
