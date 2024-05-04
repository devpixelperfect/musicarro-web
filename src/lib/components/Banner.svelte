<script>
    import { onMount } from 'svelte';
    
    export let texto = 'Texto por defecto';
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

<section class="container-fluid banner p-0">
    <div class="image-container">
        <img src="../../images/{imagen}.jpg" alt={imagen} style="transform: translateY({-scrollY * 0.4}px);">
    </div>
    <h1 class="h-100 d-flex justify-content-center align-items-center txt-blanco txt-header txt-160 lg-txt-100 md-txt-48">{texto}</h1>
</section>  

<style>

    .banner {
        position: relative;
        height: 300px;
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

    h1 {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        text-shadow: 4px 6px 5px rgb(0 0 0 / 70%);
    }

    /* h1::before {
        content: 'Gallery';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        display: flex;
        align-items: center;
        justify-content: center;
    } */

    @media only screen and (max-width: 768px) {
        .banner {
            height: 200px;
        }
        h1 {
            font-size: 48px;
        }
    }
</style>