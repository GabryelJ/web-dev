<script>
import StyledLink from "$lib/components/StyledLink.svelte";
</script>

<div class="container">
    <div class="student-list">
        <table class="student-list__table">
                <thead>
                    <tr>
                        <th>número</th>
                        <th>matricula</th>
                        <th>nome</th>
                        <th>email</th>
                    </tr>
                </thead>
            <tbody>
            <tr>
                <td>1</td>
                <td>202512345610</td>
                <td>Aluno1</td>
                <td>aluno1@grad.uni</td>
            </tr>
            <tr>
                <td>2</td>
                <td>202512345611</td>
                <td>Aluno2</td>
                <td>aluno2@grad.uni</td>
            </tr>
            <tr>
                <td>3</td>
                <td>202512345612</td>
                <td>Aluno3</td>
                <td>aluno3@grad.uni</td>
            </tr>
            <tr>
                <td>4</td>
                <td>202512345613</td>
                <td>Aluno4</td>
                <td>aluno4@grad.uni</td>
            </tr>
            <tr>
                <td>5</td>
                <td>202512345614</td>
                <td>Aluno5</td>
                <td>aluno5@grad.uni</td>
            </tr>
            <tr>
                <td>6</td>
                <td>202512345615</td>
                <td>Aluno6</td>
                <td>aluno6@grad.uni</td>
            </tr>
            <tr>
                <td>7</td>
                <td>202512345616</td>
                <td>Aluno7</td>
                <td>aluno7@grad.uni</td>
            </tr>
            <tr>
                <td>8</td>
                <td>202512345617</td>
                <td>Aluno8</td>
                <td>aluno8@grad.uni</td>
            </tr>
            <tr>
                <td>9</td>
                <td>202512345618</td>
                <td>Aluno9</td>
                <td>aluno9@grad.uni</td>
            </tr>
            <tr>
                <td>10</td>
                <td>202512345619</td>
                <td>Aluno10</td>
                <td>aluno10@grad.uni</td>
            </tr>
            </tbody>
        </table>
    </div>
    <StyledLink text="Voltar ao menu" type="button" href="/menu" />
</div>

<style>
    .container{
        display: flex;
        flex-grow: 1;
        justify-content: center;
        padding: 10px;
        flex-direction: column;
        align-items: center;
        gap: 20px;
    }

    .student-list{
        padding: 10px;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.8);
    }

    .student-list__table{
        border-collapse: collapse;
    }

    .student-list__table > thead > tr > th{
        border: 1px solid black;
        padding: 10px;
        background-color: var(--primary);
    }
    .student-list__table > tbody > tr > td{
        border: 1px solid black;
        padding: 10px;
        text-align: center;
    }
</style>