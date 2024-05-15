<script>
    import IniciarSesion from "$lib/components/formularios/IniciarSesion.svelte";
</script>
<section>
    <div  class="container py-md-5 d-flex justify-content-lg-end justify-content-center">
         <IniciarSesion />
    </div>
</section>

<style>
    section {
        background-image: url("../../images/login.jpg");
        background-size: cover;
        background-position: center;

    }
    @media screen and (max-width: 768px){
        section{
            background-image: none;
        }
    }
</style>