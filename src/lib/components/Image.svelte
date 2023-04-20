<script>
    import { lazyLoad } from '$lib/util/lazyLoad.js'

    import logo from '$lib/assets/mini.png'
    import logoweb from '$lib/assets/mini.webp'
    
    export let src = logo
    export let title = "Hmmmmm"
    export let height = "512"
    export let width = "512"
</script>

<source type="image/webp" srcset={logoweb}>
<source type="image/png" srcset={logo}>
<img use:lazyLoad={src} {height} {width} src={logo} alt={title} />