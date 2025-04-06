<script>
    import {GridAndDotBackgrounds} from "$lib/components/ui/GridAndDotBackground/index.js";
    import Robot from "$lib/models/robot_playground/robot_playground.svelte"
    import {Canvas} from "@threlte/core";
    import {OrbitControls} from '@threlte/extras'
    import {T} from '@threlte/core'
</script>

<section>

    <!--    <GridAndDotBackgrounds>-->
    <Canvas>
        <Robot></Robot>
        <T.PerspectiveCamera
                makeDefault
                position={[5, 5, 5]}
        >
            <OrbitControls/>
        </T.PerspectiveCamera>
    </Canvas>
    <!--        Hero Section-->
    <!--    </GridAndDotBackgrounds>-->


</section>