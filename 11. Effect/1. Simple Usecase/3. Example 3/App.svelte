<script>
  let score = $state(0);

  $effect(() => {
    if (score >= 5) {
      alert(`Great job! You reached a score of ${score}!`);
    }
  });
</script>

<button onclick={() => score++}>Add Point</button>
<div>Score: {score}</div>