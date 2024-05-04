<script>
    //Swiper
	import {Swiper, SwiperSlide} from 'swiper/svelte';
	import 'swiper/css';
	import 'swiper/css/navigation';
	// Swiper modulos
	import {Navigation} from 'swiper';
</script>

<section class="py-5 fdo-gris-50 px-4">
	<div class="container-fluid">
		<h2 class="txt-subtitulo mb-4 text-center anton">More products</h2>
        <p class="text-center">Pellentesque ac lobortis ipsum. <br/>
            Nullam tempor vel est imperdiet vestibulum.</p>
		<div class="row mt-5">
			<Swiper
				slidesPerView={1}
				spaceBetween={15}
				navigation={true}
				loop= {true}
				breakpoints={{
					'380': {
						slidesPerView: 2,
						spaceBetween: 8,
					},
					'769': {
						slidesPerView: 3,
						spaceBetween: 25,
					},
					'993': {
						slidesPerView: 4,
						spaceBetween: 25,
					},
					'1200': {
						slidesPerView: 4,
						spaceBetween: 30,
					},
					'1481': {
						slidesPerView: 5,
						spaceBetween: 20,
					},
				}}
				modules={[Navigation]}
				class="carrusel">

                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-3">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-2">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-2">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-2">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-2">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-2">Add to cart</button>
                    </div>
                </SwiperSlide>
                <SwiperSlide>
                    <div class="card">
                        <img src="../../images/img-producto.png" alt="">
                        <p class="mt-2 txt-20 lg-txt-18 md-txt-14">Taramp // Bajo 3K 1 OHM V2</p>
                        <button class="btn btn-rojo mt-3 px-2">Add to cart</button>
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
        padding: 20px;
        text-align: center;
    }
</style>