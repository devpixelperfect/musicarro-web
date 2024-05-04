<script>
    //Swiper
	import {Swiper, SwiperSlide} from 'swiper/svelte';
	import 'swiper/css';
	import 'swiper/css/navigation';
	// Swiper modulos
	import {Navigation, Autoplay, FreeMode} from 'swiper';
</script>

<section class="py-5 fdo-rojo px-4 txt-blanco">
	<div class="container-fluid">
		<h2 class="txt-subtitulo mb-4 text-center anton">Industry Standard</h2>
        <p class="text-center">Pellentesque ac lobortis ipsum. <br/>
            Nullam tempor vel est imperdiet vestibulum.</p>

        <div class="logos">
            <div class="logos-slide">
              <img src="../../images/img-marca.png" alt=""/>
              <img src="../../images/img-marca.png" alt=""/>
              <img src="../../images/img-marca.png" alt=""/>
              <img src="../../images/img-marca.png" alt=""/>
              <img src="../../images/img-marca.png" alt=""/>
            </div>
      
            <div class="logos-slide">
                <img src="../../images/img-marca.png" alt=""/>
                <img src="../../images/img-marca.png" alt=""/>
                <img src="../../images/img-marca.png" alt=""/>
                <img src="../../images/img-marca.png" alt=""/>
                <img src="../../images/img-marca.png" alt=""/>
            </div>
          </div>
	</div>
</section>

<style>

@keyframes slide {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-100%);
  }
}

.logos {
  overflow: hidden;
  padding: 60px 0;
  white-space: nowrap;
  position: relative;
}

.logos:before,
.logos:after {
  position: absolute;
  top: 0;
  width: 250px;
  height: 100%;
  content: "";
  z-index: 2;
}

.logos:hover .logos-slide {
  animation-play-state: paused;
}

.logos-slide {
  display: inline-block;
  animation: 15s slide infinite linear;
}

.logos-slide img {
  height: 50px;
  margin: 0 40px;
}

@media screen and (max-width: 1280px){
    .logos-slide img {
        height: 40px;
        margin: 0 40px;
    }
}
@media screen and (max-width: 768px){
    .logos-slide img {
        height: 25px;
        margin: 0 20px;
    }
    .logos {
        padding: 40px 0 20px 0;

    }
}
</style>