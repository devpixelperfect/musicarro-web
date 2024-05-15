<script>
    // export let obj = {};
    export let imagen = 'historial.jpg';
    export let titulo = 'Texto por defecto';
    export let descripcion = 'Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper';
    export let fecha = '24/01/2024';
    export let cantidad = '2';
    export let precio = '$329.00';

    // const {imagen, titulo, descripcion, fecha, cantidad, precio} = obj;
</script>

<div class="col-12 my-2">
    <div class="card">
        <div class="card-body py-3 py-lg-0 px-0 d-flex align-items-center gap-2">
            <div class="imagen">
                <img src="../../images/{imagen}" alt="">
            </div>
            <div class="d-flex flex-column gap-2 w-100">
                <h4 class="card-title anton">{titulo}</h4>
                <p class="txt-14">{descripcion}</p>
                <p class="txt-14">Date of purchase: <span class="fw-bold">{fecha}</span></p>
                <p class="txt-14">Amount: <span class="fw-bold">{cantidad}</span></p>
                <div class="d-flex gap-2">
                    <p class="fw-bold">Price</p>
                    <p class="price txt-32">{precio}</p>
                </div>
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
        max-width: 180px;
        height: 250px;
    }
    
    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
</style>