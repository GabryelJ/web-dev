<script>
    export let text = 'Botão';
    export let type = 'button';
    export let disabled = false;
    export let buttonOverWriteStyleClass = '';
</script>

<button
        {type}
        class="button {buttonOverWriteStyleClass}"
        on:click
        {disabled}
>
        {text}
</button>

<style>
    /*TODO: pensar em tipos diferentes de personalização*/
    .button{
        padding: 5px;
        font-size: 1rem;
        cursor: pointer;
        border-radius: 10px;
        background-color: var(--secondary-color);
        transition: 0.5s ease-in-out;
    }

    .button-card{
            font-weight: bold;
            width: 100px;
            height: 100px;
    }

    button:disabled {
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