<script lang="ts">
    import Telegram from '../../../node_modules/bootstrap-icons/icons/telegram.svg?raw'
    import Github from '../../../node_modules/bootstrap-icons/icons/github.svg?raw'
    import Pencil from '../../../node_modules/bootstrap-icons/icons/pencil.svg?raw'
    import Home from '../../../node_modules/bootstrap-icons/icons/house.svg?raw'

    export let name: 'telegram' | 'github' | 'home' | 'pencil', size: number = 24
    const setSize = (svg: string) => svg.replace(/=\"16\"\ /g, `=\"${size}\"\ `)
</script>

{#if name === 'telegram'}
    {@html setSize(Telegram)}
{:else if name === 'github'}
    {@html setSize(Github)}
{:else if name === 'pencil'}
    {@html setSize(Pencil)}
{:else}
    {@html setSize(Home)}
{/if}
