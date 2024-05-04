<div class="mb-5 fdo-blanco py-4 px-3 filtros">
    <h3 class="anton">Filter productos</h3>
    <p>Filter products to find results</p>

    <p class="mt-4">Category</p>
    <select class="form-select  mb-3 mt-2" aria-label="Large select example">
        <option selected>Open this select menu</option>
        <option value="1">One</option>
        <option value="2">Two</option>
        <option value="3">Three</option>
    </select>

    <p class="mt-4 mb-2">Price range</p>
    <div class="d-flex align-items-center gap-1">
        <label class="txt-12" for="volume">$100</label>
        <input class="w-100 mb-0" type="range" id="volume" name="volume" min="0" max="10000" />
        <label class="txt-12" for="volume">$10,000</label>
    </div>
    <button class="btn btn-rojo w-100 mt-4">Filter product <i class="bi bi-funnel ms-1"></i></button>
</div>

<style>
    .filtros{
        position: sticky;
        top: 100px;
    }
    
</style>