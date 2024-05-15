<script>
    // export let obj = {};
    export let imagen = 'service.jpg';
    export let titulo = 'Texto por defecto';
    export let descripcion = 'Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper';
    export let precio = '$329.00';

    // const {imagen, titulo, descripcion, precio} = obj;
</script>

<div class="col-sm-12 col-lg-6 my-2">
    <div class="card">
        <div class="card-body p-0 d-flex align-items-center">
            <div class="imagen">
                <img src="../../images/{imagen}" alt="">
            </div>
            <div class="d-flex flex-column gap-2 px-3 w-100">
                <h5 class="card-title txt-16">{titulo}</h5>
                <p>{descripcion}</p>
                <div class="d-flex gap-2">
                    <p class="fw-bold">Price</p>
                    <p class="price txt-32">{precio}</p>
                </div>
                <button class="btn btn-rojo ">Buy now</button>
            </div>
        </div>
    </div>
</div>

<style>
    .card {
        border: none;
        border-radius: 0;
    }

    .imagen {
        width: 75%;
        max-width: 220px;
        height: 230px;
    }
    
    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    h5 {
        font-family: var(--anton);
    }
</style>