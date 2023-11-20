<script lang="ts">
    import { name } from '../../../../slawenburgen/package.json'
    import { title, description } from '../../../../slawenburgen/src/app.json'
    import TableRow from './TableRow.svelte'
</script>

<TableRow {name} {description} {title} />
