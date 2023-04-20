<script>
    import Image from '$lib/components/Image.svelte'

    export let haberler
</script>

{#each haberler as haber}
<div class="card w-80 md:w-96 bg-base-100 shadow-xl image-full">
  <figure><Image src="{haber.img}" title="{haber.id}"/></figure>
  <div class="card-body">
    <h2 class="card-title">{haber.title}</h2>
    <p class="">{haber.desc}</p>
    <div class="card-actions justify-between">
      <div>
          {#each haber.tipler as tip}
          {#if tip}
          <div class="badge badge-outline">{tip}</div>
          {/if}
          {/each}
      </div>
    </div>
    <div class="card-actions justify-end">
      <button class="btn btn-info">Devamını Oku</button>
    </div>
  </div>
</div>
{/each}
