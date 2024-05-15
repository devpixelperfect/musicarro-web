<script>
    import { onMount } from 'svelte';
    
    export let texto = 'Texto por defecto';
    export let descripcion = 'Subtitle por defecto';
    export let imagen = 'banner';
    
    let scrollY = 0;
    
    onMount(() => {
        if (typeof window !== 'undefined') {
            window.addEventListener('scroll', () => {
                scrollY = window.scrollY;
            });
        }
    });
</script>

<section class="container-fluid banner p-0 ">
    <div class="image-container">
        <img src="../../images/{imagen}.jpg" alt={imagen} style="transform: translateY({-scrollY * 0.4}px);">
    </div>
    <div class="h-100 d-flex flex-column justify-content-center encabezado">
        <h1 class="d-flex justify-content-center align-items-center txt-blanco txt-header txt-160 lg-txt-100 md-txt-48">{texto}</h1>
        <span class="txt-blanco d-flex justify-content-center align-items-center txt-header txt-20">{descripcion}</span>
        <div class="barra mt-2 mx-auto"></div>
    </div>
</section>  

<style>
    .banner {
        position: relative;
        height: 400px;
        overflow: hidden;
    }

    .image-container {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    img {
        width: 100%;
        height: 200%;
        object-fit: cover;
        position: relative;
    }

    .encabezado {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
    }

    span {
        margin-top: -10px;
    }

    .barra {
        width: 10%;
        height: 5px;
        border-radius: 5px;
        background-color: var(--color-blanco);
    	box-shadow: 0px 3px 2.6px 0px rgba(0, 0, 0, 0.48) inset;
        filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    }

    @media only screen and (max-width: 768px) {
        .banner {
            height: 200px;
        }
    }
</style>
