<script>
    export let text = 'Botão';
    export let type = 'button';
    export let variant = 'primary';
    export let disabled = false;
</script>

<button
        {type}
        class="button {variant}" on:click{onClickFunction}
        on:click
        {disabled}
>
        {text}
</button>

<style>
    /*TODO: pensar em tipos diferentes de personalização*/
    .button{
        padding: 5px;
        font-size: 1em;
        cursor: pointer;
        border-radius: 10px;
    }
    .primary {
        background-color: var(--secondary-color);
        transition: 0.5s ease-in-out;
    }
    .primary:hover {
        background-color: var(--primary-color);
        transform: scale(0.96);
        box-shadow: 0 1px 0 #575353;
    }

</style>