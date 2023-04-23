<script>

    import Nav from '$lib/components/Nav.svelte'
    import Header from "$lib/components/Header.svelte";
    import MobileHeader from "$lib/components/HeaderMobile.svelte";
    import Footer from "$lib/components/Footer.svelte";

</script>

<svelte:head>
<title>Hypixel - The Minecraft Server</title>
</svelte:head>

<div class="drawer">
    <input id="sidemenu" aria-label="toggle-drawer" type="checkbox" class="drawer-toggle" /> 
    <div class="drawer-content flex flex-col">
        <Header />
        <Nav />
        <MobileHeader />
        <slot />
        <Footer />
    </div> 
    <div class="drawer-side">
      <label for="sidemenu" class="drawer-overlay"></label> 
      <ul class="menu p-4 w-80 bg-base-100">
        <li><a href="/login">Log in</a></li>
        <li><a href="/signin">Sign in</a></li>
      </ul>
    </div>
  </div>