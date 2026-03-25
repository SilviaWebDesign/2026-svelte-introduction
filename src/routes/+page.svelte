
<script>

    import ClicksCounter from "$lib/components/ClicksCounter.svelte";
    import ProgressiveSum from "$lib/components/ProgressiveSum.svelte";

    let count = $state(5)
</script>


<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<ClicksCounter initialCount={5} />
<p> count from parent: {count}</p>

<style>
    h1 {
        color: rgb(21, 42, 195);
    }
</style>
