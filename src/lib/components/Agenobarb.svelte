<script lang="ts">
    import { name } from '../../../../agenobarb/package.json'
    import { title, description } from '../../../../agenobarb/src/app.json'
    import TableRow from './TableRow.svelte'
</script>

<TableRow {name} {description} {title} />
