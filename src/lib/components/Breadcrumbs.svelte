<script>
	import { each } from "svelte/internal";

    export let items = []
</script>

<div class="text-sm breadcrumbs btn">
    <ul>
        {#each items as item}
        {#if item.href}
        <li><a href={item.href ? item.href : "#"}>{item.name}</a></li>
        {:else}
        <li>{item.name}</li>
        {/if}
        {/each}
    </ul>
</div>