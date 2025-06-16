<script>
  let firstName = $state('Alex');
  let lastName = $state('Mercer');

  let fullName = $derived(`${firstName} ${lastName}`);
</script>

<h1>{fullName}</h1>

<input bind:value={firstName} placeholder="First name" />
<input bind:value={lastName} placeholder="Last name" />
