<section class="py-5">
    <div class="container py-5">
        <h2 class=" anton">
            Our happy clients
        </h2>
        <p>Pellentesque ac lobortis ipsum. <br/>
            Nullam tempor vel est imperdiet vestibulum.</p>
        <div class="comentario mt-5 p-md-5 p-3 d-flex gap-md-5 gap-3 align-items-center">
            <p class="txt-160 md-txt-48 anton">“</p>
            <p class="txt-24 lg-txt-18 md-txt-16">Nunc ut justo erat. Donec at eros vehicula, vestibulum tellus in, dignissim massa. Nunc et faucibus felis. Ut consectetur ipsum ut ligula placerat rutrum. Ut sit amet tristique magna, interdum molestie tellus.</p>
        </div>
        <div class="marcador">
            <svg class="marcador" xmlns="http://www.w3.org/2000/svg" width="120" height="59" viewBox="0 0 120 59" fill="none">
                <path d="M35.0002 58.5L-2.51516e-06 -2.86134e-06L120 1.14441e-05L35.0002 58.5Z" fill="white"/>
            </svg>
        </div>
        
        <div class="d-flex justify-content-between mt-2 gap-2 align-items-center">
            <div>
                <img src="../../images/img-testimonial.png" alt="">
            </div>
            <div class="d-flex gap-2 align-items-center">
                <img src="../../images/img-testimonial.png" alt="">
                <div>
                    <h3 class="anton">Sara Jonson</h3>
                    <p class="md-txt-12">Pellentesque ac lobortis ipsum. </p>
                </div>
            </div>
            <div>
                <img src="../../images/img-testimonial.png" alt="">
            </div>
            <div>
                <img src="../../images/img-testimonial.png" alt="">
            </div>
        </div>
    </div>
</section>

<style>
    img{
        width: 160px;
    }
    .comentario {
        box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.4);
    }
    .marcador svg{
        filter: drop-shadow(0px 5px 3px rgba(0,0,0,0.3));
        margin-top: -2px;

    }
    .marcador{
        display: flex;
        justify-content: end;
        width: 50%;
    }
    .txt-160{
        max-height: 130px;
    }
    @media screen and (max-width: 1280px){
        img{
            width: 130px;
        }
    }
    @media screen and (max-width: 992px){
        img{
            width: 100px;
        }
    }
    @media screen and (max-width: 768px){
        img{
            width: 60px;
        }
    }
    @media screen and (max-width: 580px){
        img{
            width: 40px;
        }
        .marcador svg{
            margin-top: -4px;
            min-width: 105px !important;

        }
    }
</style>