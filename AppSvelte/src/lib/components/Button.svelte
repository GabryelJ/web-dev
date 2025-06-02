<script>
    export let text = 'Botão';
    export let type = 'button';
    export let disabled = false;
    export let variant = '';
    export let href = undefined;
</script>

{#if href}
        <a
                href={href}
                class="button {variant}"
                on:click
                {disabled}
        >
                {text}
        </a>
{:else}

        <button
                {type}
                class="button {variant}"
                on:click
                {disabled}
        >
                {text}
        </button>
{/if}

<style>
    .button{
        padding: 5px;
        font-size: 1rem;
        cursor: pointer;
        border-radius: 10px;
        background-color: var(--secondary-color);
        transition: 0.5s ease-in-out;
        text-decoration: none;
        color: black;
        border: 1px solid black;
        display: inline-flex;
        justify-content: center;
        align-items: center;
        font-weight: bold;
    }

    a.button{
            font-size: 1.1rem;
    }

    .button-card{
            width: 100px;
            height: 100px;
            text-align: center;
    }

    .button:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            background-color: #cccccc;
            color: #666666;
    }

    .button:hover {
        background-color: var(--primary-color);
        transform: scale(0.96);
        box-shadow: 0 2px 0 #ccc;
    }

    .button-exit{
            background-color: var(--exit);
            font-weight: bold;
            padding: 10px 10px;
    }
    .button-exit:hover{
            background-color: var(--secondary-color);
            transform: scale(0.94);
    }

</style>