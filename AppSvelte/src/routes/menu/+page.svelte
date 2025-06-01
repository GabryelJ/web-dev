<script>
import Button from "$lib/components/Button.svelte";
</script>

<div class="flex-container">
    <div class="menu">
        <Button text="Grade horária docente" type="button" buttonOverWriteStyleClass="button-card"></Button>
        <Button text="Alunos com matrícula ativa" type="button" buttonOverWriteStyleClass="button-card"></Button>
        <Button text="Diário de aulas" type="button" buttonOverWriteStyleClass="button-card"></Button>
        <Button text="Registro de notas e faltas" type="button" buttonOverWriteStyleClass="button-card"></Button>
        <Button text="Ementário" type="button" buttonOverWriteStyleClass="button-card"></Button>
    </div>
    <Button text="Sair" type="button" buttonOverWriteStyleClass="button-exit"></Button>
</div>

<style>
    .flex-container{
        display: flex;
        flex-grow: 1;
        flex-direction: column;
        gap: 40px;
        align-items: center;
        justify-content: center;
    }
    .menu {
        display: flex;
        flex-wrap: wrap;
        background-color: var(--secondary-color);
        padding: 20px;
        border-radius: 10px;
        border: 1px solid black;
        gap: 10px;
        justify-content: center;
    }
</style>