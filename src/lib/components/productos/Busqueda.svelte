<div class="d-flex mt-4 w-100 gap-2 flex-sm-nowrap flex-wrap justify-content-sm-between justify-content-start">
    <div class="input-group">
        <input type="text" class="form-control" placeholder="Buscar..." aria-label="Buscar..." aria-describedby="button-addon2">
        <button class="btn btn-outline-secondary fdo-gris px-3" type="button" id="button-addon2">
            <i class="bi bi-search"></i>
        </button>
    </div>

    <select class="form-select mt-sm-0 mt-5 " aria-label="Large select example">
        <option selected>Order by</option>
        <option value="1">One</option>
        <option value="2">Two</option>
        <option value="3">Three</option>
    </select>
</div>

<style>
    .btn{
        border: 1px solid var(--color-gris-900);
        border-left: none !important;
        border-radius: 0px !important;
    }
    .btn-outline-secondary:hover{
        background-color: var(--color-rojo);
        border: 1px solid var(--color-gris-900);
        
    }
    input{
        border-right: none !important;
        max-width: 350px;
    }
    select{
        width: 140px;
    }

    @media screen and (max-width: 576px){
        input{
            max-width: 100%;
        }
    }
</style>