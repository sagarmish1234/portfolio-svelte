<script lang="ts">
    import Hero from "$lib/components/Hero.svelte";
    import Education from "$lib/components/Education.svelte";
    import ShortProfile from "$lib/components/ShortProfile.svelte";
    import Experience from "$lib/components/Experience/Experience.svelte";
</script>


<svelte:head>
    <title>Sagar Mishra</title>
    <meta name="description" content="Sagar Mishra's portfolio"/>
</svelte:head>


<section>
    <Hero></Hero>
    <Education/>
    <Experience/>
    <!--    <ShortProfile></ShortProfile>-->
</section>

<style>
</style>
