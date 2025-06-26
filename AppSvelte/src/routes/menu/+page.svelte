<script>
import Button from "$lib/components/Button.svelte";
import StyledLink from "$lib/components/StyledLink.svelte";
</script>

<div class="flex-container">
    <div class="menu">
        <StyledLink text="Grade horária docente" type="button" variant="button-card" href="/grade-horaria"></StyledLink>
        <StyledLink text="Alunos com matrícula ativa" type="button" variant="button-card" href="/alunos-ativos"></StyledLink>
        <StyledLink text="Diário de aulas" type="button" variant="button-card"></StyledLink>
        <StyledLink text="Registro de notas e faltas" type="button" variant="button-card"></StyledLink>
        <StyledLink text="Ementário" type="button" variant="button-card"></StyledLink>
    </div>
    <StyledLink text="Sair" type="button" variant="button-exit" href="."></StyledLink>
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
        gap: 10px;
        justify-content: center;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.8);
    }
</style>