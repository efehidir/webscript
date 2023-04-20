<script>
    import "../app.css";

    import { onMount } from 'svelte'
    import { themeChange } from 'theme-change'

    import Nav from '$lib/components/Nav.svelte'
    import Header from "../lib/components/Header.svelte";
    import MobileHeader from "../lib/components/HeaderMobile.svelte";
    import Footer from "../lib/components/Footer.svelte";

    onMount(() => {
      themeChange(false)
    })
</script>

<svelte:head>
<title>Hypixel - The Minecraft Server</title>
</svelte:head>

<Header />
<Nav />
<MobileHeader />
<slot />
<Footer />