<script>
import ScheduleTable from "$lib/components/ScheduleTable.svelte";
import Button from "$lib/components/Button.svelte";
</script>


<div class="container">
    <ScheduleTable></ScheduleTable>
    <Button text="Voltar ao menu" type="button"/>
</div>


<style>
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        flex-grow: 1;
        gap: 20px;
        margin: 25px 0;
    }
</style>