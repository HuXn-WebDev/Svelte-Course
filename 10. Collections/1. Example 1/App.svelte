<script>
    const friends = ['alex', 'bob', 'charlie', 'dave', 'eve'];
</script>

<div>
    <h1>Friends List</h1>
    <ul>
        {#each friends as friend}
            <li>{friend}</li>
        {/each}
    </ul>
</div>

