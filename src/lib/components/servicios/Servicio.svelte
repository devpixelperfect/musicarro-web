<script>
    // export let obj = {};
    export let imagen = 'service.jpg';
    export let titulo = 'Texto por defecto';
    export let descripcion = 'Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper ';
    export let precio = '$329.00';

    // const {image, titulo, descripcion, precio} = obj;
</script>

<div class="d-flex flex-column flex-md-row gap-4">
    <div class="imagen">
        <img src="../../images/{imagen}" alt="">
    </div>
    <div class="d-flex flex-column gap-3 justify-content-center">
        <h2 class="txt-32">{titulo}</h2>
        <p>{descripcion}</p>
        <div class="d-flex justify-content-between">
            <div>
                <span class="txt-32 fw-bold">200+</span>
                <p class="fw-bold">Characteristics</p>
            </div>
            <div>
                <span class="txt-32 fw-bold">34+</span>
                <p class="fw-bold">Characteristics</p>
            </div>
            <div>
                <span class="txt-32 fw-bold">97%+</span>
                <p class="fw-bold">Characteristics</p>
            </div>
        </div>
        <div class="d-flex gap-2">
            <p class="fw-bold">Price</p>
            <p class="price txt-40">{precio}</p>
        </div>
        <button class="btn btn-rojo">Buy now</button>
    </div>
</div>

<style>
    .imagen {
        width: 70%;
        max-width: 600px;
    }

    @media only screen and (max-width: 992px) {
        .imagen {
            width: 100%;
            max-width: 100%;
        }
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    h2 {
        font-family: var(--anton);
    }
</style>