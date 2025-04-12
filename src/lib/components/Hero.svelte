<script>
    import {GridAndDotBackgrounds} from "$lib/components/ui/GridAndDotBackground/index.js";
    import Header from "./Header.svelte"
    import Bot from "$lib/models/robot_playground/bot.svelte"
    import {Canvas} from "@threlte/core";
    import {T} from '@threlte/core'
    import TypewriterEffect from "$lib/components/ui/TypewriterEffect/TypewriterEffect.svelte";
</script>

<section>

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
    <section class="text-white jetbrains-mono-400 w-full px-52 pt-24 flex flex-col gap-8 mt-32">
        <div class="text-5xl ">Hello I am</div>
        <div class="text-6xl">Sagar Mishra</div>
        <TypewriterEffect></TypewriterEffect>
    </section>


</section>

<style>
    @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,100..800;1,100..800&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100..900;1,100..900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    .jetbrains-mono-400 {
        font-family: "JetBrains Mono", monospace;
        font-optical-sizing: auto;
        font-weight: 400;
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