<script>
	import Productos from "$lib/components/carrusel/Productos.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import ProductosDestacados from "$lib/components/carrusel/ProductosDestacados.svelte";
    import GridDestacados from "$lib/components/utilidades/GridDestacados.svelte";
    import Testimoniales from "$lib/components/utilidades/Testimoniales.svelte";
    import SlideHome from "$lib/components/slides/SlideHome.svelte";
	import Mapa from "$lib/components/utilidades/Mapa.svelte";
	
	
	
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<SlideHome />
	<GridDestacados />
	<Mapa />

	
</section>

<style>

</style>
