<script lang="ts">
    import '../app.css';

    let {children} = $props();

</script>

<div class="app">

    <main>
        {@render children()}
    </main>

</div>

<style>
    .app{
        background-color: #0a0909;
        min-height: 100vh;
    }
</style>
