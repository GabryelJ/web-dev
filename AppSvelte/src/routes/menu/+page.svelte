<script>
import Button from "$lib/components/Button.svelte";
</script>

<div class="flex-container">
    <div class="menu">
        <Button text="Grade horária docente" type="button" variant="button-card" href="/grade-horaria"></Button>
        <Button text="Alunos com matrícula ativa" type="button" variant="button-card"></Button>
        <Button text="Diário de aulas" type="button" variant="button-card"></Button>
        <Button text="Registro de notas e faltas" type="button" variant="button-card"></Button>
        <Button text="Ementário" type="button" variant="button-card"></Button>
    </div>
    <Button text="Sair" type="button" variant="button-exit" href="/"></Button>
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
        padding: 20px;
        border-radius: 10px;
        border: 1px solid black;
        gap: 10px;
        justify-content: center;
    }
</style>