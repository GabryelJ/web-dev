<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import Input from "$lib/components/Input.svelte";
    import Button from "$lib/components/Button.svelte";
    import LoginForm from "$lib/components/LoginForm.svelte";

</script>

<main class="flex-container">
    <Header/>
    <div class="login">
        <LoginForm />
    </div>
    <Footer/>
</main>


<style>
    @import '../lib/styles/app.css';
    .flex-container {
        display: flex;
        flex-direction: column;
        height: 100vh;
    }
    .login {
        display: flex;
        flex-grow: 1;
        align-items: center;
        justify-content: center;
    }
</style>

