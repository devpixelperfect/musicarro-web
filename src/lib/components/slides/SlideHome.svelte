<div class="slide">
    <div class="d-flex justify-content-center">
        <h1 class="anton text-uppercase txt-blanco txt-160">Car Audio</h1>
    </div>
    <div class="container d-flex justify-content-between">
        <div class="d-flex gap-lg-3 w-50">
            <div class="position-relative d-flex justify-content-center">
                <div class="btn-slide d-flex justify-content-center uno">
                    <h4 class="txt-blanco rotar txt-uno">Car audio</h4>
                </div>
            </div>
            
            <div class="position-relative d-flex justify-content-center">
                <div class="btn-slide d-flex justify-content-center dos">
                    <h4 class="txt-blanco rotar txt-dos">Remote start</h4>
                </div>
            </div>
        </div>
        <div class="cont-img">
            <img src="../../images/slide/car-audio.png" alt="" class="w-100">
        </div>
        <div class="d-flex gap-lg-3 w-50 justify-content-end">
            <div class="position-relative d-flex justify-content-center">
                
                <div class="btn-slide d-flex justify-content-center tres">
                    <h4 class="txt-blanco rotar txt-tres">Car security</h4>
                </div>
            </div>
            
            <div class="position-relative d-flex justify-content-center">
                
                <div class="btn-slide d-flex justify-content-center cuatro">
                    <h4 class="txt-blanco rotar txt-cuatro">Dash camera</h4>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    .slide{
        background-image: url('../../../images/slide-musicarro.jpg');
        background-position: center;
        height: 550px;
        background-repeat: no-repeat;
    }
    .container{
        margin-top: -60px;
    }
    .btn-slide{
        background-color: var(--color-rojo);
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 3px solid var(--color-blanco);
        transition: all 0.5s;
    }
    .btn-slide:hover {
        background-color: var(--color-blanco);
        border: 3px solid var(--color-gris-900);
        
    }
    .cont-img{
       min-width: 680px;
    }
    /*Botones*/
    .rotar{
        transform: rotate(-90deg);
        position: absolute;
        width: max-content;
        transition: all 0.5s;
        opacity: 0;
    }
    .uno, .cuatro{
        margin-top: 70px;
    }
    .txt-uno{
        top: 0px;
    }
    .dos, .tres{
        margin-top: 120px;
    }
    .txt-dos{
        top: 30px;
    }
    .txt-tres{
        top: 40px;
    }
    .txt-cuatro{
        top: -15px;
    }
    /*Hovers Botones*/
    .uno:hover .txt-uno{
        opacity: 1;
    }
    .dos:hover .txt-dos{
        opacity: 1;
    }
    .tres:hover .txt-tres{
        opacity: 1;
    }
    .cuatro:hover .txt-cuatro{
        opacity: 1;
    }

    @media (max-width: 1400px){
        .slide{
            background-position: center -55px;
        }
    }

    @media (max-width: 1200px){
        .slide{
            height: 450px;
            background-position: center -100px;
        }
        .cont-img{
            min-width: 500px;
        }
        .btn-slide{
            width: 80px;
            height: 80px;
        }
    }
    @media (max-width: 992px){
        .txt-160{
            font-size: 100px;
        }
        .cont-img{
            min-width: 400px;
        }
        .btn-slide{
            width: 70px;
            height: 70px;
        }
        .slide{
            height: 350px;
            background-position: center -190px;
            padding-top: 20px;
        }
    }
</style>