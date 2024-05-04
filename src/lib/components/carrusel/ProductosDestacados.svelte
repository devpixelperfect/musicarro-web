<script>
    //Swiper
	import {Swiper, SwiperSlide} from 'swiper/svelte';
	import 'swiper/css';
	import 'swiper/css/navigation';
	// Swiper modulos
	import {Navigation, FreeMode} from 'swiper';
</script>

<section class="py-5 fdo-gris-50 px-4">
	<div class="container">
		<h2 class="txt-subtitulo mb-4 text-center anton">Best products</h2>
        <p class="text-center">Pellentesque ac lobortis ipsum. <br/>
            Nullam tempor vel est imperdiet vestibulum.</p>
		<div class=" mt-5 d-flex align-items-center">
			<Swiper
				slidesPerView={1}
				spaceBetween={15}
				navigation={true}
				loop= {true}
				breakpoints={{
                    '300': {
						slidesPerView: 1,
						spaceBetween: 10,
					},
					'600': {
						slidesPerView: 3,
						spaceBetween: 10,
					},
					'769': {
						slidesPerView: 3,
						spaceBetween: 25,
					},
					'993': {
						slidesPerView: 3,
						spaceBetween: 25,
					},
					'1200': {
						slidesPerView: 3,
						spaceBetween: 30,
					},
					'1481': {
						slidesPerView: 3,
						spaceBetween: 20,
					},
				}}
				modules={[Navigation]}
				class="destacados">

                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 ">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3">Add to cart</button>
                    </div>
                </SwiperSlide>

			</Swiper>
		</div> 
	</div>
</section>

<style>
    .card{
        background-color: #fff;
        border-radius: 0px;
        padding: 40px 20px 0px 20px;
        text-align: center;
        /* transition: all 1s; */
        /* border: none; */
    }
    /* .card:hover p, .card:hover button{
        display: block;
        opacity: 1;
    }
    .card:hover{
        border: 1px solid #000;
        padding-top: 60px;
        padding-bottom: 60px;
    } */
    .card p{

        opacity: 0;
        /* transition: all 1s; */
    }
    .card button{
        opacity: 0;
        /* transition: all 1s; */
    }

    @media screen and (max-width: 768px){
        .container{
            max-width: 100%;
            padding-left: 0px;
            padding-right: 0px;
        }
    }
</style>