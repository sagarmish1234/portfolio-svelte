<script lang="ts">
    import {cn} from "$lib/utils/cn";

    export let showFade: boolean = true;

</script>

<div
        class={cn(
    "absolute inset-5" +
     " bg-[#0f0f0f] ",
    "[background-size:40px_40px]",
    "[background-image:linear-gradient(to_right,#e4e4e7_1px,transparent_1px),linear-gradient(to_bottom,#e4e4e7_1px,transparent_1px)]",
    "dark:[background-image:linear-gradient(to_right,#262626_1px,transparent_1px),linear-gradient(to_bottom,#262626_1px,transparent_1px)]",
    "-z-10"
    )}
>
    <!-- Radial gradient for the container to give a faded look -->
    {#if showFade}
        <div class="pointer-events-none  absolute inset-0 flex items-center justify-center bg-white [mask-image:radial-gradient(ellipse_at_center,transparent_50%,black)] dark:bg-black"></div>
    {/if}
    <slot/>
</div>

<style lang="postcss">

</style>
