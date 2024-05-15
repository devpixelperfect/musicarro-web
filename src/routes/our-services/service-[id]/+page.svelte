<script>
    import Banner from "$lib/components/banners/Banner.svelte";
	import Breadcrumb from "$lib/components/utilidades/Breadcrumb.svelte";
	import Servicio from "$lib/components/servicios/Servicio.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Productos from "$lib/components/carrusel/Productos.svelte";
</script>

<!-- Banner component -->
<Banner texto="Our Services" imagen="banner"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <Breadcrumb link="our-services" section="Bajo 3K 1 OHM V2"/>
        <Servicio title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam neque ultrices." price="329.00"/>
    </div>
</section>

<!-- Secciones adicionales -->
<Marcas/>
<Productos/>