<script>
    // export let obj = {};
    export let image = 'service.jpg';
    export let title = 'Texto por defecto';
    export let description = 'Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper ';
    export let price = '$329.00';

    // const {image, title, description, price} = obj;
</script>


    <div class="d-flex flex-column gap-3 justify-content-center cont-info">
        <h2 class="txt-32 anton">{title}</h2>
        <p>{description}</p>
        <div class="d-sm-flex justify-content-between">
            <div>
                <span class="txt-32 fw-bold">200+</span>
                <p class="fw-bold">Characteristics</p>
            </div>
            <div class="mt-sm-0 mt-3">
                <span class="txt-32 fw-bold">34+</span>
                <p class="fw-bold">Characteristics</p>
            </div>
            <div class="mt-sm-0 mt-3">
                <span class="txt-32 fw-bold">97%+</span>
                <p class="fw-bold">Characteristics</p>
            </div>
        </div>
        <div class="d-sm-flex justify-content-between align-items-center mb-xl-5 mb-3">
            <div>
                <label for="exampleFormControlInput1" class="form-label">Amount</label>
                <input type="number" class="form-control" id="exampleFormControlInput1" placeholder="0">
            </div>
            <div class="d-flex gap-2 mt-sm-0 mt-4">
                <p class="fw-bold">Price</p>
                <p class="price txt-40">{price}</p>
            </div>
        </div>
        <div class="d-sm-flex gap-2">
            <button class="btn btn-rojo w-100">Add to cart</button>
            <button class="btn btn-transparente-blanco w-100 mt-sm-0 mt-3">Buy now</button>
        </div> 
    </div>

<style>
    input{
        max-width: 180px;
    }
  
</style>