<script>
    import Banner from "$lib/components/banners/Banner.svelte";
	import Titulo from "$lib/components/utilidades/Titulo.svelte";
	import CardServicio from "$lib/components/servicios/Card-servicio.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Productos from "$lib/components/carrusel/Productos.svelte";
</script>

<!-- Banner component -->
<Banner texto="Our Services" imagen="banner"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <div class="d-flex justify-content-between">
            <Titulo/>
                <select class="form-select">
                    <option selected>Order by</option>
                    <option value="1">Order A-Z</option>
                    <option value="2">Order Z-A</option>
                </select>
        </div>

        <div class="row my-4">
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
            <CardServicio titulo="Remote Starter Installation" descripcion="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" precio="329.00"/>
        </div>
    </div>
</section>

<!-- Secciones adicionales -->
<Marcas/>
<Productos/>

<style>
    .form-select{
        width: min(150px, 100%);
    }
</style>
