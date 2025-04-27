<script lang="ts">
    import '../app.css';
    export const prerender = true;
    let {children} = $props();

</script>

<div class="app">

    <main>
        {@render children()}
    </main>

</div>

<style>

</style>
