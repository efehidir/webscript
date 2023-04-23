<script>
  import logo from '$lib/assets/big.png'
  import bg from '$lib/assets/bg.jpg'
  import logoweb from '$lib/assets/big.webp'
  import bgweb from '$lib/assets/bg.webp'
</script>

<div class="hero h-60 hidden md:grid" style="background-image: url({bg});">
  <div class="hero-overlay bg-opacity-80"></div>
  <div class="hero-content text-neutral-content">
        <picture>
          <source type="image/webp" srcset={logoweb}>
          <source type="image/png" srcset={logo}>
          <img class="max-w-sm rounded-lg" height="256" width="512" draggable="false" src={logo} alt="hypixel_logo">
        </picture>
        <p class="py-6">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint distinctio excepturi deserunt exercitationem, iste magni quos omnis quo fugit, asperiores necessitatibus minus esse error saepe illum nostrum molestiae. Ipsam, minima.</p>
        <button class="btn btn-info">Lorem Ipsum</button>
  </div>
</div>
