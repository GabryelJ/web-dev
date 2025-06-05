<script>
    import { page } from '$app/state';
    import Button from '$lib/components/Button.svelte';

    const status = $derived(page.status);
    const error = $derived(page.error);
    const title = $derived(page.status === 404 ? 'Página não encontrada' : 'Erro inesperado');
    const message = $derived(
        page.status === 404
            ? 'A página que você tentou acessar não existe.'
            : (page.error?.message || 'Algo deu errado.')
    );
</script>

<main class="error-container">
    <div class="error-content">
        <h1>{status}: {title}</h1>
        <p>{message}</p>

        {#if status !== 404 && error?.stack}
            <pre>{error.stack}</pre>
        {/if}

        <Button text="Voltar para a página inicial" href="/" />
    </div>
</main>

<style>
    .error-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        text-align: center;
        padding: 20px;
    }

    .error-content {
        background-color: white;
        padding: 40px;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        max-width: 600px;
        width: 100%;
    }

    h1 {
        color: var(--primary);
        font-size: 2.5rem;
        margin-bottom: 20px;
    }

    p {
        font-size: 1.1rem;
        margin-bottom: 30px;
    }

    pre {
        background-color: #eee;
        padding: 15px;
        border-radius: 5px;
        overflow-x: auto;
        text-align: left;
        white-space: pre-wrap;
        word-break: break-all;
        margin-top: 20px;
    }
</style>
