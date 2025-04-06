<script>
    import {GridAndDotBackgrounds} from "$lib/components/ui/GridAndDotBackground/index.js";
    import Header from "./Header.svelte"
    // import Robot from "$lib/models/robot_playground/robot_playground.svelte"
    import Bot from "$lib/models/robot_playground/bot.svelte"
    import {Canvas} from "@threlte/core";
    // import {OrbitControls} from '@threlte/extras'
    import {T} from '@threlte/core'
</script>

<section>

    <Header></Header>
    <GridAndDotBackgrounds>
        <!--        Hero Section-->
        <Canvas>
            <T.AmbientLight color="#ffffff" intensity={0.2}/>
            <T.DirectionalLight
                    color="#ffffff"
                    intensity={2}
                    position={[10, 10, 0]}
                    shadow.camera.top={8}
                    castShadow
            />
            <!--            <Robot position={[1.75,.3,0]} scale={0.8}></Robot>-->
            <Bot position={[40.75,-10.3,-100]} scale={0.25}></Bot>
            <T.PerspectiveCamera
                    makeDefault
                    position={[0, 1, 5]}
            >
                <!--                <OrbitControls/>-->
            </T.PerspectiveCamera>
        </Canvas>
    </GridAndDotBackgrounds>


</section>