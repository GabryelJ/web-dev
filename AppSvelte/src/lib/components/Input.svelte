<script>
    let {
        value = "",
        label = 'legenda',
        placeholder = 'Ex.: placeholder',
        type = 'text',
        direction = '',
        labelLinkId = ''
    } = $props();
</script>

<div class="labeled-input {direction}">
    <label class="label" for="{labelLinkId}">
        {label}
    </label>
    <input class="input" id="{labelLinkId}"
           {type}
           {placeholder}
           bind:value
    >
</div>

<style>
    .labeled-input {
        display: flex;
    }

    .column{
        flex-direction: column;
    }

    .label {
        margin-top: 10px;
        margin-bottom: 5px;
        font-weight: bold;
        font-size: 1rem;
    }

    .input {
        padding: 5px;
        font-size: 1rem;
        width: 100%;
        border-radius: 10px;
        border: 1px solid black;
        transition: border-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
    }

    .input:focus {
        box-shadow: 0 0 0 3px rgb(0, 128, 198);
    }
</style>