<script>
    import Navbar from '../components/navbar.svelte'
</script>

<style>
    @import '/css/global.css';
</style>

<Navbar />
<main>
    <slot />
</main>