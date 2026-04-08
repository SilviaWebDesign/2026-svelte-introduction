<script>
    let todos = $state([
        {title: "Assigmnet 1", done: false},
        {title: "Assigmnet 2", done: false},
        {title: "Assigmnet 3", done: false},
    ])
</script>

<h3>Todos</h3>

<ul>
    {#each todos as todo}
        <li>
            <input type="checkbox" bind:checked={todo.done}>
            (todo.title)
        </li>
    {/each}
</ul>