<script>
    let { initialCount: count }= $props();

    // let count = $state(initialCount);
    let doubled = $derived(count* 2)

</script>


<h3>Clicks counter</h3>

  
<button onclick={() => count++}>
    Clicks: {count}
</button>

<span> doubled is {doubled} </span>

