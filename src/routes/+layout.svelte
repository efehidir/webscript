<script>
    import "../app.css";

    import { onMount } from 'svelte'
    import { themeChange } from 'theme-change'

    onMount(() => {
      themeChange(false)
    })
</script>

<svelte:head>
<title>Hypixel - The Minecraft Server</title>
</svelte:head>

<slot />