<!--TODO: funcionalidades-->
<script>
    import Input from "$lib/components/Input.svelte";
    import Button from "$lib/components/Button.svelte";

    let registratiomNumber = "";
    let password = "";
</script>

<form class="login-container">
    <Input label="Matrícula:" type="text" direction="column" bind:value={registratiomNumber} placeholder="Ex.: 202510033011"/>
    <Input label="Senha:" type="password" direction="column" bind:value={password} placeholder="••••••••"/>
    <hr>
    <div class="buttons">
        <Button text="Entrar" type="submit" variant="primary" />
        <Button text="Esqueci a Senha" type="button" variant="primary" />
        <Button text="Cadastro" type="button" variant="primary" />
    </div>
</form>

<style>
    .login-container{
        display: flex;
        flex-direction: column;
        background-color: var(--secondary-color);
        padding: 10px;
        border-radius: 10px;
        border: 1px solid black;
    }

    hr{
        margin-top: 15px;
        margin-bottom: 15px;
    }

    .buttons{
        display: flex;
        flex-direction: column;
        gap: 10px;
    }
</style>