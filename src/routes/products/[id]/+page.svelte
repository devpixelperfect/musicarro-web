<script>
    import Banner from "$lib/components/Banner.svelte";
	import Breadcrumb from "$lib/components/Breadcrumb.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Productos from "$lib/components/carrusel/Productos.svelte";
    import Informacion from "$lib/components/productos/Informacion.svelte";
    import Producto from "$lib/components/carrusel/Producto.svelte";
</script>

<!-- Banner component -->
<Banner texto="Car audio" imagen="car-audio"/>

<section class="fdo-blanco-50 py-5">
    <div class="container mb-5">
        <Breadcrumb link="our-services" section="Bajo 3K 1 OHM V2"/>
        <div class="d-flex flex-column flex-md-row gap-lg-4 gap-2">
            <Producto />
            <Informacion title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam neque ultrices." price="329.00"/>
        </div>
       
    </div>
    <Marcas />
    <Productos />
</section>

<style>
    @media screen and (max-width: 992px){
        .container{
            max-width: 100%;
            padding-left: 30px;
            padding-right: 30px;
        }
    }
    @media only screen and (max-width: 540px) {
        .container {
            padding-left: 15px;
            padding-right: 15px;
        }
    }
</style>

