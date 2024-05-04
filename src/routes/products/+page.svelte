<script>
	import Productos from "$lib/components/carrusel/Productos.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Filtros from "$lib/components/products/Filtros.svelte";
    import Categorias from "$lib/components/products/Categorias.svelte";
    import Busqueda from "$lib/components/products/Busqueda.svelte";
    import Tienda from "$lib/components/products/Tienda.svelte";
    
    
	let innerWidth = 0;
	$: console.log(innerWidth);
</script>

<svelte:window bind:innerWidth />

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="fdo-gris-50">
    <div class="fdo-gris-500 py-5">
        <div class="container d-flex justify-content-center">
            <h1 class="txt-160 lg-txt-40">
                Slide
            </h1>
        </div>
    </div>
	
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
	<Productos />
</section>

<style>
    @media screen and (max-width: 1200px){
        .container{
            max-width: 100%;
        }
    }
</style>
