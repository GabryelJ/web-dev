<script>
    const scheduleJson = {
        "turmas":[
        {
            "codigo":"ABC99-00001",
            "nome":"Introdução a apertar botão",
            "turma":1,
            "horarios":[
                "SEG M1M2",
                "QUA M1M2"
            ]
        },
        {
            "codigo":"ABC99-00002",
            "nome":"Introdução a impressoras",
            "turma":1,
            "horarios":[
                "TER M1M2",
                "QUI M1M2"
            ]
        },
        {
            "codigo":"ABC99-00003",
            "nome":"Introdução a ar-condicionado",
            "turma":1,
            "horarios":[
                "TER M3M4",
                "SEX M3M4"
            ]
        },
        {
            "codigo":"ABC99-00004",
            "nome":"Interpretação de códigos de erro",
            "turma":1,
            "horarios":[
                "SEG M3M4",
                "SEX M1M2"
            ]
        }
    ]
    }
</script>

<div class="container">
    <table class="table">
        <thead>
            <tr>
                <th>Tempo</th>
                <th>Segunda</th>
                <th>Terça</th>
                <th>Quarta</th>
                <th>Quinta</th>
                <th>Sexta</th>
                <th>Sábado</th>
                <th>Domingo</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td class="time">M1 (07:00 - 07:50)</td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
            </tr>
            <tr>
                <td class="time">M2 (07:50 - 08:40)</td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
            </tr>
            <tr>
                <td class="time">M3 (08:50 - 09:40)</td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
            </tr>
            <tr>
                <td class="time">M4 (09:40 - 10:30)</td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
            </tr>
            <tr>
                <td class="time">M5 (10:40 - 11:30)</td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
            </tr>
            <tr>
                <td class="time">M6 (11:30 - 12:20)</td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
                <td class="morning"></td>
            </tr>
            <tr>
                <td class="time">T1 (12:30 - 13:20)</td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
            </tr>
            <tr>
                <td class="time">T2 (13:20 - 14:10)</td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
            </tr>
            <tr>
                <td class="time">T3 (14:20 - 15:10)</td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
            </tr>
            <tr>
                <td class="time">T4 (15:10 - 16:00)</td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
            </tr>
            <tr>
                <td class="time">T5 (16:10 - 17:00)</td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
            </tr>
            <tr>
                <td class="time">T6 (17:00 - 17:50)</td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
                <td class="afternoon"></td>
            </tr>
            <tr>
                <td class="time">N1 (18:00 - 18:50)</td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
            </tr>
            <tr>
                <td class="time">N2 (18:50 - 19:40)</td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
            </tr>
            <tr>
                <td class="time">N3 (19:40 - 20:30)</td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
            </tr>
            <tr>
                <td class="time">N4 (20:30 - 21:20)</td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
            </tr>
            <tr>
                <td class="time">N5 (21:20 - 22:10)</td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
                <td class="night"></td>
            </tr>
        </tbody>
    </table>
</div>


<style>
    .container {
        padding: 10px;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.8);
    }
    .table{
        border-collapse: collapse;
    }

    .table > thead > tr > th {
        border: 1px solid black;
        padding: 5px;
        min-width: 120px;
        background-color: var(--primary);
    }
    .table > tbody > tr > td {
        border: 1px solid black;
        padding: 5px;
    }

    .time{
        font-weight: bold;
    }

    .morning{
        background-color: #faf687;
    }

    .afternoon{
        background-color: lightsalmon;
    }

    .night{
        background-color: lightskyblue;
    }
</style>