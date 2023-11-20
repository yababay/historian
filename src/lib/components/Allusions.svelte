<script lang="ts">
    import { name } from '../../../../allusions/package.json'
    import { title, description } from '../../../../allusions/src/app.json'
    import TableRow from './TableRow.svelte'
</script>

<TableRow {name} {description} {title} />
