<script>
	import Productos from "$lib/components/carrusel/Productos.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Filtros from "$lib/components/productos/Filtros.svelte";
    import Categorias from "$lib/components/productos/Categorias.svelte";
    import Busqueda from "$lib/components/productos/Busqueda.svelte";
    import Tienda from "$lib/components/productos/Tienda.svelte";
    import BannerDos from "$lib/components/Banner-dos.svelte";
    
    
	let innerWidth = 0;
	$: console.log(innerWidth);
</script>

<svelte:window bind:innerWidth />

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="fdo-gris-50">
    <BannerDos texto= "All products" descripcion="Musicarro"/>
	
    <div class="container mt-5">
        <div class="d-flex gap-xl-5 gap-4">
            
            {#if innerWidth > 992}
                <div class="w-25">
                    <Filtros />
                </div>
            {/if}
            
            <div class="cont tienda" class:w-75={innerWidth > 992}>
                <Categorias />
                <Busqueda />
                <Tienda />
            </div>
        </div>
    </div>

	<Marcas />
	<!-- <Productos /> -->
</section>

<style>
    @media screen and (max-width: 1200px){
        .container{
            max-width: 100%;
        }
    }
</style>
