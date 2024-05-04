<script>
    import Banner from "../../lib/components/Banner.svelte";
	import Title from "../../lib/components/Title.svelte";
	import CardService from "../../lib/components/servicios/Card-service.svelte";
</script>

<!-- Banner component -->
<Banner texto="Our Services" imagen="banner"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <div class="d-flex justify-content-between">
            <Title/>
                <select class="form-select">
                    <option selected>Order by</option>
                    <option value="1">Order A-Z</option>
                    <option value="2">Order Z-A</option>
                </select>
        </div>

        <div class="row my-4">
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
            <CardService title="Remote Starter Installation" description="Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper" price="329.00"/>
        </div>
    </div>
</section>

<style>
    .form-select{
        width: min(150px, 100%);
    }
</style>
