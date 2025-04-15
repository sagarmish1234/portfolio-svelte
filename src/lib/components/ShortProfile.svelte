<script lang="ts">

    import BentoGrid from './ui/BentoGrid/BentoGrid.svelte';
    import BentoGridItem from './ui/BentoGrid/BentoGridItem.svelte';
    import Icon from "@iconify/svelte";
    import IMG1 from "$lib/images/bento-1.jpg";

</script>

<div class="flex items-center justify-center">
    <Icon icon="iconamoon:profile" width="35" height="35" class="text-[#00D492]"/>
    <h1 class="text-white text-center text-3xl">Profile</h1>
</div>
<BentoGrid className="max-w-4xl mx-auto md:auto-rows-[20rem] mt-10">

    <BentoGridItem className="col-span-2 bg-[url($lib/images/bento-1.jpg)]" >
        <img src={IMG1} alt="img" class="rounded-xl object-contain ">
        <div class="text-white p-4">
            Hello World
        </div>

    </BentoGridItem>

</BentoGrid>