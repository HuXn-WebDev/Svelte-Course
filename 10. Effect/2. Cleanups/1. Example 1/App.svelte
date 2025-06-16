<script>
  let seconds = $state(0);

  $effect(() => {
    const timer = setInterval(() => {
      seconds += 1;
    }, 1000);

    return () => clearInterval(timer); 
  });
</script>

<div>Seconds passed: {seconds}</div>