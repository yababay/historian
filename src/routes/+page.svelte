<script lang="ts">
    import Agenobarb from "$lib/components/Agenobarb.svelte"
    import Allusions from "$lib/components/Allusions.svelte"
    import AngryAbba from "$lib/components/AngryAbba.svelte"
    import Slawenburgen from "$lib/components/Slawenburgen.svelte"
</script>

<table class="table table-secondary table-striped">
    <thead>
        <tr>
            <th>Проект</th>
            <th>Описание</th>
            <th>Действия</th>
        </tr>
    </thead>
    <tbody>
        <Agenobarb />
        <Allusions />
        <AngryAbba />
        <Slawenburgen />
    </tbody>
</table>

<style lang="scss">
    table {
        max-width: 100ch;
        margin: 0 auto;
    }
</style>

