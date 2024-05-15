<script>
    import CrearCuenta from "$lib/components/formularios/CrearCuenta.svelte";

    CrearCuenta
</script>
<section>
    <div  class="container py-md-5 d-flex justify-content-lg-start justify-content-center">
         <CrearCuenta />
    </div>
</section>

<style>
    section {
        background-image: url("../../images/create-account.jpg");
        background-size: cover;
        background-position: center;

    }
    @media screen and (max-width: 768px){
        section{
            background-image: none;
        }
    }
</style>