<script>
	import Productos from "$lib/components/carrusel/Productos.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import ProductosDestacados from "$lib/components/carrusel/ProductosDestacados.svelte";
    import GridDestacados from "$lib/components/utilidades/GridDestacados.svelte";
    import Testimoniales from "$lib/components/utilidades/Testimoniales.svelte";
	
	
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<div class="container d-flex justify-content-center">
		<h1 class="mt-5 txt-160 lg-txt-40">
			Contenido
		</h1>
	</div>
	<GridDestacados />
	<ProductosDestacados />
	<Testimoniales />
	<Marcas />
	<Productos />
</section>

<style>

</style>
