<script>
    import {GridAndDotBackgrounds} from "$lib/components/ui/GridAndDotBackground/index.js";
    import Header from "./Header.svelte"
    import Bot from "$lib/models/robot_playground/bot.svelte"
    import Resume from "$lib/assests/CV_Sagar_Mishra_2025.pdf"
    import {Canvas} from "@threlte/core";
    import Icon from "@iconify/svelte";
    import {T} from '@threlte/core'
    import TypewriterEffect from "$lib/components/ui/TypewriterEffect/TypewriterEffect.svelte";
</script>

<section class="min-h-screen">

    <!--    <Header></Header>-->
    <GridAndDotBackgrounds>
        <Canvas>
            <T.AmbientLight color="#ffffff" intensity={0.2}/>
            <T.DirectionalLight
                    color="#ffffff"
                    intensity={2}
                    position={[10, 10, 0]}
                    shadow.camera.top={8}
                    castShadow
            />
            <Bot position={[30.75,0.3,-100]} scale={0.25} rotation="{[0,-.35,0]}"></Bot>
            <T.PerspectiveCamera
                    makeDefault
                    position={[0, 1, 5]}
            >
            </T.PerspectiveCamera>
        </Canvas>
    </GridAndDotBackgrounds>
    <!--    Jumbotron-->
    <section class=" jetbrains-mono-400 w-full px-52 pt-24 flex flex-col gap-8 mt-24">
        <div class="text-3xl text-white ">Hello I'm</div>
        <div class="text-6xl text-white">Sagar Mishra</div>
        <TypewriterEffect></TypewriterEffect>

        <div class="mt-14 flex items-center gap-10">
            <a download="CV_Sagar_Mishra_2025.pdf" target="_blank" href={Resume}>
                <button
                        class="hover:bg-[#00D492] transition duration-200 text-emerald-400 border px-5 py-4 rounded-4xl hover:text-black hover:cursor-pointer">
                    Download CV
                </button>
            </a>
            <div class="border rounded-2xl h-10 w-10 border-[#00D492] flex items-center justify-center">
                <a href="https://www.linkedin.com/in/sagar-mishra-76b990198/" target="_blank">
                    <Icon icon="eva:linkedin-fill" width="24" height="24" class="text-[#00D492]"/>
                </a>
            </div>
            <div class="border rounded-2xl h-10 w-10 border-[#00D492] flex items-center justify-center">
                <a href="https://github.com/sagarmish1234" target="_blank">
                    <Icon icon="ri:github-fill" width="24" height="24" class="text-[#00D492]"/>
                </a>
            </div>
            <div class="border rounded-2xl h-10 w-10 border-[#00D492] flex items-center justify-center">
                <a href="https://leetcode.com/u/sagarmish1234/" target="_blank">
                    <Icon icon="tabler:brand-leetcode" width="24" height="24" class="text-[#00D492]"/>
                </a>
            </div>
        </div>
    </section>


</section>

<style>
    @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,100..800;1,100..800&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100..900;1,100..900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    .jetbrains-mono-400 {
        font-family: "JetBrains Mono", monospace;
        font-optical-sizing: auto;
        font-weight: 600;
        font-style: normal;
    }


    .raleway-400 {
        font-family: "Raleway", sans-serif;
        font-optical-sizing: auto;
        font-weight: 400;
        font-style: normal;
    }

    .montserrat-400 {
        font-family: "Montserrat", sans-serif;
        font-optical-sizing: auto;
        font-weight: 400;
        font-style: normal;
    }


    .montserrat-600 {
        font-family: "Montserrat", sans-serif;
        font-optical-sizing: auto;
        font-weight: 600;
        font-style: normal;
    }

</style>