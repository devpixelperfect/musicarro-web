<script>
    import RecuperarCotrasenia from "$lib/components/formularios/RecuperarCotrasenia.svelte";
    
</script>
<section>
    <div  class="container py-md-5 d-flex justify-content-lg-end justify-content-center">
         <RecuperarCotrasenia />
    </div>
</section>

<style>
    section {
        background-image: url("../../../images/reset.jpg");
        background-size: cover;
        background-position: center;

    }
    @media screen and (max-width: 768px){
        section{
            background-image: none;
        }
    }
</style>