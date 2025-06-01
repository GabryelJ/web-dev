<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import "$lib/styles/app.css";
</script>

<div class="flex-container">
    <Header />

    <slot />

    <Footer />
</div>

<style>
    @import '../lib/styles/app.css';
    .flex-container {
        display: flex;
        flex-direction: column;
        min-height: 100vh;
    }
</style>