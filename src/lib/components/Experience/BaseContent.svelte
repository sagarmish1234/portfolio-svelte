<script>

    import {cn} from "$lib/utils/cn.js";

    const {company, className,timeline} = $props();


</script>

<div>
    <h1 class={cn("text-3xl mb-5" ,className)}>{company}</h1>
    <h2 class="text-[#00D492] text-2xl">{timeline}</h2>
    <div>
        <slot/>
    </div>
</div>