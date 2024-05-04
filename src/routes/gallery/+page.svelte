<script>
    import Banner from "../../lib/components/Banner.svelte";
</script>

<!-- Banner component -->
<Banner texto="Gallery" imagen="gallery"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <div class="grid-container">
            <!-- Grid superior -->
            <div class="grid-item">
                <img src="../../images/gallery/gallery-1.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-2.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-3.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-4.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-5.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-6.jpg" alt="">
            </div>

            <div class="grid-item">
                <img src="../../images/gallery/gallery-7.jpg" alt="">
            </div>

            <!-- Grid inferior -->
            <div class="grid-item">
                <img src="../../images/gallery/gallery-8.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-9.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-10.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-11.jpg" alt="">
            </div>
            <div class="grid-item">
                <img src="../../images/gallery/gallery-12.jpg" alt="">
            </div>
        </div>
    </div>
</section>

<style>
    .grid-container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-auto-rows: minmax(240px, auto);
        grid-gap: 20px;
    }

    .grid-item:nth-child(1) { grid-row: span 3; grid-column: span 2; }
    .grid-item:nth-child(4) { grid-column: span 2; }

    .grid-item:nth-child(7) { grid-column: span 4; grid-row: span 2;}

    .grid-item:nth-child(8) { grid-column: span 2; }
    .grid-item:nth-child(9) { grid-column: span 2; grid-row: span 3; }
    .grid-item:nth-child(10) { grid-row: span 2;}

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    @media only screen and (max-width: 768px) {
        .grid-container {
            grid-template-columns: 1fr; 
            grid-gap: 10px;
        }

        .grid-item:nth-child(1),
        .grid-item:nth-child(4),
        .grid-item:nth-child(7),
        .grid-item:nth-child(8),
        .grid-item:nth-child(9),
        .grid-item:nth-child(10) {
            grid-column: 1; 
            grid-row: auto; 
        }
    }
</style>