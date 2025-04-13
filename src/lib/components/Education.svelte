<script>
    import Icon from "@iconify/svelte";
    import MagicCard from "$lib/components/ui/MagicCard.svelte";
</script>

<section class="h-[75vh]">
    <div class="flex justify-center">
        <Icon icon="carbon:education" width="40" height="40" class="text-[#00D492]"/>
        <h1 class="text-white text-4xl ">Education</h1>
    </div>
    <section class="flex gap-10 justify-center px-20 mt-16">

        <MagicCard
                class="cursor-pointer shadow-2xl whitespace-nowrap text-4xl group hover:border-[#00D492] transition-all duration-300 size-1/4 h-max min-h-64"
                gradientColor="#043634"
                gradientSize={100}
        >
            <div class="p-5 flex flex-col gap-5">

                <h1 class="text-sm">Class X </h1>
                <p class="text-xl"> Birla Bharati </p>
                <p class="text-sm">May, 2015 - May, 2016</p>
                <div class="flex items-center gap-2">
                    <Icon icon="qlementine-icons:education-16" width="20" height="20" class="text-[#00D492]"/>
                    <h1 class="text-[#00D492] text-lg">10.00 CGPA</h1>
                </div>
            </div>
        </MagicCard>
        <MagicCard
                class="cursor-pointer shadow-2xl whitespace-nowrap text-4xl group hover:border-[#00D492] transition-all duration-300 size-1/4 h-max min-h-64"
                gradientColor="#043634"
                gradientSize={100}
        >
            <div class="p-5 flex flex-col gap-5">

                <h1 class="text-sm">Higher Secondary </h1>
                <p class="text-xl"> Birla Bharati </p>
                <p class="text-sm">May, 2016 - June, 2018</p>
                <div class="flex items-center gap-2">
                    <Icon icon="qlementine-icons:education-16" width="20" height="20" class="text-[#00D492]"/>
                    <h1 class="text-[#00D492] text-lg">93.80 %</h1>
                </div>
            </div>
        </MagicCard>
        <MagicCard
                class="cursor-pointer shadow-2xl whitespace-nowrap text-4xl group hover:border-[#00D492] transition-all duration-300 size-1/4 h-max min-h-56"
                gradientColor="#043634"
                gradientSize={100}
        >
            <div class="p-5 flex flex-col gap-5">

                <h1 class="text-sm">Bachelor of Technology</h1>
                <p class="text-xl text-wrap"> Veer Surendra Sai University of Technology </p>
                <p class="text-sm">Aug, 2018 - June, 2022</p>
                <div class="flex items-center gap-2">
                    <Icon icon="qlementine-icons:education-16" width="20" height="20" class="text-[#00D492]"/>
                    <h1 class="text-[#00D492] text-lg">9.02 CGPA</h1>
                </div>
            </div>
        </MagicCard>
    </section>
</section>