<script lang="ts">
    import Icon from "./Icon.svelte"

    export let name: string, title: string, description: string, editable: boolean = true
    const href = `https://github.com/yababay/${name}`
    const home = `http://${name}.yababay.me`
    const articles = `https://github.com/yababay/${name}/tree/articles`
</script>
<tr>
    <td><a target="_blank" {href} {title}>{name}</a></td>
    <td>{description}</td>
    <td>
        <div class="icon-holder">
            <a href={home}><Icon name="home" /></a>
            {#if editable}
                <a href={articles}><Icon name="pencil" /></a>
            {/if}
        </div>
    </td>
</tr>

<style>
    .icon-holder {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-around;
    }
</style>
