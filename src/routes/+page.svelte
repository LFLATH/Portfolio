<script>
    import Logo from "../components/logo.svelte";
    import Hero from "../components/hero.svelte"
</script>


<div class="page_container">
    <Logo></Logo>
    <Hero></Hero> 
</div>



<style>
    .page_container {
        font-family: 'Baumans', cursive;;
    }
    .page_container {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
    }
</style>