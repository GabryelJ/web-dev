<script>
    import Input from "$lib/components/Input.svelte";
    import Button from "$lib/components/Button.svelte";

    let registrationNumber = $state("");
    let password = $state("");

    function isEmpty(field) {
        return field.trim() === "";
    }

    let loginDisabled = $derived(isEmpty(registrationNumber) || isEmpty(password));

</script>

<form class="login-container">
    <div class="inputs-container">
        <Input label="Matrícula:" type="text" direction="column" labelLinkId="matricula" bind:value={registrationNumber} placeholder="Insira sua matrícula"/>
        <Input label="Senha:" type="password" direction="column" labelLinkId="senha" bind:value={password} placeholder="Insira sua senha"/>
    </div>

    <div class="buttons">
        <Button text="Entrar" type="submit" disabled={loginDisabled}/>
        <hr>
        <Button text="Esqueci minha senha" type="button"/>
        <Button text="Cadastro" type="button"/>
    </div>
</form>

<style>
    .login-container{
        display: flex;
        flex-direction: column;
        background-color: var(--secondary);
        padding: 10px;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.8);
    }

    .inputs-container {
        margin-bottom: 20px;
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