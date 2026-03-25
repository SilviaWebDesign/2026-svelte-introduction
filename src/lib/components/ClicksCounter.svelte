<script>

    let count = $state(0)
    let doubled = $derived(count* 2)

</script>


<h3>Clicks counter</h3>


<button on:click={() => count++}>
    clicks: {count}
</button>

<span> doubled is {doubled} </span>