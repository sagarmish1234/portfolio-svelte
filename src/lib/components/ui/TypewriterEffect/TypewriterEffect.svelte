<script>
    import TypeIt from "typeit";
    import {onMount} from "svelte";

    let ref = $state();


    onMount(() => {
        new TypeIt(ref, {speed: 130})
            .type("soft",{delay:500})
            .move(-3)
            .delete(1)
            .type("S",{delay:100})
            .move(3,{delay:300})
            .type("ware eng")
            .move(-2)
            .delete(1)
            .type("E")
            .move(3)
            .type("ineer")
            .go();
    })

</script>


<div bind:this={ref} class="text-emerald-400 text-5xl">

</div>
