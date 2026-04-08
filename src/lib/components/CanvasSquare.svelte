<script>
    import {untrack} from "svelte"

    let size= $state(50)
    let color= $state("#ff3e00")

    let canvas 

    $effect(() => {
        const context = canvas.getContext("2d")
        context.clearRect(0,0, canvas.width, canvas.height)

        context.fillStyle = untrack(() => color)
        context.fillRect(0,0, size, size)
    })

    // let canvas = document.querySelector("canvas")
    
    // on mounth - montato pronto
    // effect - reazione

</script>

<h3>Canvas Square</h3>

<article>
    <canvas bind:this={canvas} width="100" height="100"></canvas>

    <nav>
        <label>
            Size: <input type="range" bind:value={size}>
        </label>

         <label>
            Color: <input type="color" bind:value={color}>
        </label>
    </nav>
</article>

<style>
    article {
        display: flex;
        gap: len;
        align-items: flex-end;
    }

    canvas {
        border: solid 1px black;
    }

    nav {
        display: flex;
        gap: len;
        flex-direction: column;
    }
</style>