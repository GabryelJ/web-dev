<script>
     let {
        text = 'Botão',
        type = 'button',
        disabled = false,
        variant = '',
     } = $props();
</script>



<button {type} class="button {variant}" onclick={""} {disabled}>
        {text}
</button>


<style>
    .button{
        padding: 5px;
        font-size: 1rem;
        cursor: pointer;
        border-radius: 10px;
        background-color: var(--secondary);
        transition: 0.5s ease-in-out;
        text-decoration: none;
        color: black;
        border: 1px solid black;
        display: inline-flex;
        justify-content: center;
        align-items: center;
        font-weight: bold;
    }

    .button:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            background-color: #cccccc;
            color: #666666;
    }

    .button:hover {
        background-color: var(--primary);
        transform: scale(0.96);
        box-shadow: 0 2px 0 #ccc;
    }


</style>