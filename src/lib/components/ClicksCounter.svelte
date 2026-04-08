<script>
    let { initialCount }= $props();

    // let count = $state(initialCount);
    let doubled = $derived(initialCount* 2)


</script>


<h3>Clicks counter</h3>

  
<button onclick={() => initialCount++}>
    Clicks: {initialCount}
</button>

<span> doubled is {doubled} </span>

