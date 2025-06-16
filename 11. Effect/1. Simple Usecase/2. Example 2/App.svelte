<script>
  let username = $state('Guest');

  $effect(() => {
    document.title = `Welcome, ${username}!`;
  });
</script>

<input type="text" bind:value={username} placeholder="Enter your name" />