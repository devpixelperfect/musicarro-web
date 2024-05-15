<script>
	//Swiper
	import {Swiper, SwiperSlide} from 'swiper/svelte';
	import 'swiper/css';
	import 'swiper/css/thumbs';

	import {page} from '$app/stores';
	//Manejar errores


	import {FreeMode, Navigation, Thumbs} from 'swiper';
	// Swiper modulos

	let thumbsSwiper = null;

	const setThumbsSwiper = (e) => {
		const [swiper] = e.detail;
		// set Thumbs swiper instance
		setTimeout(() => {
			thumbsSwiper = swiper;
		});
	};
</script>

<div class="d-flex align-self-center align-items-center flex-lg-row flex-column-reverse">
	<div class="w-100 overflow-hidden">
		<Swiper
			on:swiper={setThumbsSwiper}
			spaceBetween={24}
			slidesPerView={5}
			freeMode={true}
			watchSlidesProgress={true}
			modules={[FreeMode, Navigation, Thumbs]}
			direction="vertical"
			class="miniaturas"
			breakpoints={{
				'0': {
					slidesPerView: 3,
					spaceBetween: 60,
					direction: 'horizontal',
				},
				'430': {
					slidesPerView: 4,
					spaceBetween: 25,
					direction: 'horizontal',
				},
				'769': {
					direction: 'horizontal',
					slidesPerView: 5,
					spaceBetween: 20,
				},
				'993': {
					direction: 'vertical',
                    
				},
			}}>
			
            <SwiperSlide><div class="thumb-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
            <SwiperSlide><div class="thumb-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
            <SwiperSlide><div class="thumb-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
            <SwiperSlide><div class="thumb-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
            <SwiperSlide><div class="thumb-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
            <SwiperSlide><div class="thumb-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
				
		</Swiper>
	</div>
	<div class="w-100 overflow-lg-visible overflow-lg-hidden position-relative">
		<Swiper
			navigation={false}
			thumbs={{swiper: thumbsSwiper}}
			modules={[FreeMode, Navigation, Thumbs]}
			direction="horizontal"
			slidesPerView={1}
			spaceBetween={32}
			breakpoints={{
				0: {
					direction: 'horizontal',
				},
				768: {
					direction: 'horizontal',
				},
			}}
			class="galeria">
				<SwiperSlide><div class="img-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>
                <SwiperSlide><div class="img-galeria"><img class="w-100" src="../../images/img-producto.png" /></div></SwiperSlide>

		</Swiper>
		
	</div>
</div>

<style>
	.thumb-galeria {
		width: 90px;
		height: 90px;
		border-radius: 10px;
		overflow: hidden;
		border: 2px solid var(--color-blanco);
		box-shadow: 0px 3px 10px #00000019;
	}
	.img-galeria {
		width: 100%;
		height: 100%;
		overflow: hidden;
		/* box-shadow: 0px 3px 10px #00000019; */
	}
	img {
		width: 100%;
		height: 100%;
		object-fit: cover !important;
		object-position: center !important;
	}



	@media only screen and (max-width: 1400px) {
		/* .img-galeria {
			width: 520px;
			height: 450px;
		} */

		.thumb-galeria {
			width: 70px;
			height: 70px;
		}
	}
	@media only screen and (max-width: 1200px) {


		.thumb-galeria {
			width: 55px;
			height: 55px;
		}
	}
	@media only screen and (max-width: 992px) {
		.thumb-galeria {
			width: 70px;
			height: 70px;
		}
		/* .img-galeria {
			width: 100%;
            max-width: 350px;
			height: 350px;
		} */
	}

	@media only screen and (max-width: 768px) {
		/* .img-galeria {
			height: 280px;
		} */
        
	}

	@media only screen and (max-width: 540px) {
		/* .img-galeria {
			height: 240px;
		} */
	}
</style>
