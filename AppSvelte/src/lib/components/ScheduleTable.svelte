<script>
    const days = ["Segunda", "Terça", "Quarta", "Quinta", "Sexta", "Sábado"];

    const times = [
        { id: "M1", label: "M1 (07:00 - 07:50)" },
        { id: "M2", label: "M2 (07:50 - 08:40)" },
        { id: "M3", label: "M3 (08:50 - 09:40)" },
        { id: "M4", label: "M4 (09:40 - 10:30)" },
        { id: "M5", label: "M5 (10:40 - 11:30)" },
        { id: "M6", label: "M6 (11:30 - 12:20)" },
        { id: "T1", label: "T1 (12:30 - 13:20)" },
        { id: "T2", label: "T2 (13:20 - 14:10)" },
        { id: "T3", label: "T3 (14:20 - 15:10)" },
        { id: "T4", label: "T4 (15:10 - 16:00)" },
        { id: "T5", label: "T5 (16:10 - 17:00)" },
        { id: "T6", label: "T6 (17:00 - 17:50)" },
        { id: "N1", label: "N1 (18:00 - 18:50)" },
        { id: "N2", label: "N2 (18:50 - 19:40)" },
        { id: "N3", label: "N3 (19:40 - 20:30)" },
        { id: "N4", label: "N4 (20:30 - 21:20)" },
        { id: "N5", label: "N5 (21:20 - 22:10)" },
    ];

    let schedule = {
        "M5": { "Terça": "Matéria 1", "Quinta": "Matéria 1" },
        "M6": { "Terça": "Matéria 1", "Quinta": "Matéria 1" },
    };
</script>


<table>
    <thead>
    <tr>
        <th>Tempo</th>
        {#each days as day}
            <th>{day}</th>
        {/each}
    </tr>
    </thead>
    <tbody>
    {#each times as time}
        <tr>
            <td class="time-label">{time.label}</td>
            {#each days as day}
                <td class:cell-filled={schedule[time.id]?.[day]}>
                    {schedule[time.id]?.[day]}
                </td>
            {/each}
        </tr>
    {/each}
    </tbody>
</table>


<style>
    table {
        border-collapse: collapse;
        text-align: center;
    }

    th, td {
        border: 2px solid #373737;
        padding: 3px;
    }

    .time-label {
        font-weight: bold;
        background-color: var(--secondary-color);
    }

</style>