<script>
    let props = $props()
    let count = $state(props.initialCount)
    let doubled = $derived(count* 2)

    console.log("hello world")
</script>


<h3>Clicks counter</h3>


<button on:click={() => count++}>
    clicks: {count}
</button>

<span> doubled is {doubled} </span>