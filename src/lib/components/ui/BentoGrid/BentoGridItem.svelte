<script lang="ts">
    import {cn} from '$lib/utils/cn';

    export let className: string | undefined = undefined;
</script>

<div
        class={cn(
		'group/bento row-span-1 flex flex-col justify-between rounded-xl border border-transparent bg-white  shadow-input transition duration-200 hover:shadow-xl dark:border-white/[0.2] dark:bg-black dark:shadow-none',className
	)}
>
    <slot name="header"/>
    <div class="transition duration-200 group-hover/bento:translate-x-2">
        <slot/>
    </div>
</div>