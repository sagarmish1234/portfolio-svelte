<script>
    import Timeline from "$lib/components/ui/Timeline/Timeline.svelte";

    import Icon from "@iconify/svelte";
    import Content1 from "$lib/components/Experience/Content1.svelte";
    import Content2 from "$lib/components/Experience/Content2.svelte";


    let timelineData = [
        {
            title: "Software Engineer",
            content: Content1,
        },
        {
            title: "Intern",
            content: Content2,
        }
    ];
</script>

<div>
    <div class="flex justify-center items-center">
        <Icon icon="material-symbols-light:work-outline" width="50" height="50" class="text-[#00D492]"/>
        <h1 class="text-white text-4xl">Experience</h1>
    </div>
    <Timeline {timelineData}/>
</div>
