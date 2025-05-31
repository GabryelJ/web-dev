<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import Button from "$lib/components/Button.svelte";
</script>

<main class="flex-container">
    <Header></Header>
    <div class="login">
        
    </div>
    <Footer></Footer>
</main>


<style>
    @import '../lib/styles/app.css';
    .flex-container {
        display: flex;
        flex-direction: column;
        height: 100vh;
    }
    .login {
        flex-grow: 1;
    }
</style>

