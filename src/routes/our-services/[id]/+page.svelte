<script>
    import Banner from "../../../lib/components/Banner.svelte";
	import Breadcrumb from "../../../lib/components/Breadcrumb.svelte";
	import Service from "../../../lib/components/servicios/Service.svelte";
</script>

<!-- Banner component -->
<Banner texto="Our Services" imagen="banner"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <Breadcrumb link="our-services" section="Bajo 3K 1 OHM V2"/>
        <Service title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam neque ultrices." price="329.00"/>
    </div>
</section>

