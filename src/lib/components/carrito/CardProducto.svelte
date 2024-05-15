<div class=" d-flex fdo-blanco gap-2 align-items-center position-relative px-3 py-3">
    <i class="bi bi-x txt-32"></i>
    <div class="img-producto fdo-blanco">
        <img class="" src="../../images/img-producto.png" alt="">
    </div>
    <div class="w-100">
        <h5 class="anton mt-2 pe-4">Taramp // Bajo 3K 1 OHM V2</h5>
        <p class="mt-2 txt-14 lg-txt-12">Lorem ipsum dolor sit amet consectetur turpis ornare dolor diam arcu semper </p>
        <div class="d-flex justify-content-between align-items-center mt-4">
            <input type="number" class="form-control text-center" id="exampleFormControlInput1" placeholder="0" value="2">
            <h2 class=""> <span class="anton">$200.00</span></h2>
        </div>
       
    </div>
</div>

<style>
    .img-producto {
        width: 200px;
        height: 200px;
        min-width: 200px;
        min-height: 200px;
    }
    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    input{
        max-width: 100px;
    }
    .bi{
        position: absolute;
        right: 10px;
        top: 10px;
        cursor: pointer;
    }

    @media (max-width: 992px){
        .img-producto {
            width: 150px;
            height: 150px;
            min-width: 150px;
            min-height: 150px;
        }
    }
    @media (max-width: 768px){
        .img-producto {
            width: 100px;
            height: 100px;
            min-width: 100px;
            min-height: 100px;
        }
    }
    @media only screen and (max-width: 540px) {
        .img-producto {
            width: 80px;
            height: 80px;
            min-width: 80px;
            min-height: 80px;
        }
        input{
            max-width: 70px;
        }
        .bi{
            position: absolute;
            right: 10px;
            top: 0px;
            cursor: pointer;
        }
    }

</style>