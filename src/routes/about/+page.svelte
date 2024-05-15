<script>
	import BannerDos from "$lib/components/banners/Banner-dos.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Productos from "$lib/components/carrusel/Productos.svelte";
</script>

<!-- Banner component -->
<BannerDos texto="About us" descripcion="27 YEARS AGO IT ALL STARTED" imagen="about"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <div class="d-flex flex-column gap-5 m-auto">
            <p class="text-center">
                Lorem ipsum dolor sit amet consectetur. Ullamcorper ultrices integer et eget consectetur mattis phasellus odio. Neque aliquam pulvinar consectetur lorem velit egestas. Commodo facilisis ultricies urna in mollis consectetur. Scelerisque sed id amet nisl. Aliquam in justo massa etiam urna vulputate non. Lectus porttitor curabitur amet adipiscing. Neque amet felis eu aenean viverra blandit aliquet sit faucibus. Et nunc eu sed cursus mauris erat. Vitae diam augue mollis sit faucibus erat pretium. Lorem pharetra vulputate commodo est velit.
            </p>
            <p class="text-center">
                Non purus elementum orci in ac ullamcorper tortor odio. Sed sit varius cras vulputate in elit. Convallis pharetra faucibus sapien eget placerat. Eget aliquet dolor mi gravida id nunc erat. Diam leo habitant velit iaculis nunc turpis elementum. Duis tincidunt donec eget a in amet elementum interdum pretium. Dis cras pharetra porttitor aliquam amet lacus mollis sit. Adipiscing dolor blandit tortor duis et sit in. Blandit vestibulum fringilla in pretium adipiscing turpis semper
            </p>
        </div>
    </div>
</section>

<!-- Secciones adicionales -->
<Marcas/>
<Productos/>

<style>
    div {
        width: 70%;
    }

    @media only screen and (max-width: 768px) {
        div {
            width: 100%;
        }
    }
</style>