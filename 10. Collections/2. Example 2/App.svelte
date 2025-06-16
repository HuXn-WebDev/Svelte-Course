<script>
    const movies = [
        { title: "Inception", year: 2010, },
        { title: "The Matrix", year: 1999 },
        { title: "Interstellar", year: 2014, },
        { title: "The Godfather", year: 1972,  },
        { title: "Pulp Fiction", year: 1994, }
    ]
</script>


<section>
    <h1>Movie List</h1>
    <ul>
        {#each movies as movie}
            <li>{movie.title} ({movie.year})</li>
        {/each}
    </ul>
</section>
