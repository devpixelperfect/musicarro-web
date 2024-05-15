<script>
    import CardProducto from "$lib/components/carrito/CardProducto.svelte";
    import Orden from "$lib/components/carrito/Orden.svelte";
</script>
<section>
    <div>
        <div class="container py-4">
            <h2 class="anton">Shopping cart</h2>
        </div>
    </div>
    <div class="fdo-gris-50">
        <div class="container py-5">
            <div class="row">
                <div class="col-lg-8 col-md-7">
                    <CardProducto />
                    <hr>
                    <CardProducto />
                    <hr>
                    <CardProducto />
                    <hr>
                    <CardProducto />
                </div>
                <div class="col-lg-4 col-md-5 mt-md-0 mt-5">
                    <Orden />
                </div>
            </div>
    </div>
</section>

<style>
    hr{
        border: 1px solid #000;
        margin: 25px 0;
    }

    @media (max-width: 992px){
        .container {
            max-width: 100% !important;
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