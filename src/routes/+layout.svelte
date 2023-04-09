<style>
    h1 
    {
        font-weight: 100;
        font-size: 3rem;
    }
</style>

<h1>Svelte Site</h1>
<Navbar />

<slot></slot>

<script>
    import Navbar from './Navbar.svelte';
</script>