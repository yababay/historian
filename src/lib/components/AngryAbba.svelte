<script lang="ts">
    import { name } from '../../../../angry-abba/package.json'
    import { title, description } from '../../../../angry-abba/src/app.json'
    import TableRow from './TableRow.svelte'
</script>

<TableRow {name} {description} {title} />
