<script>
	let innerWidth = 0;
	$: console.log(innerWidth);
</script>

<svelte:window bind:innerWidth />

<header class="fdo-rojo txt-blanco d-flex align-items-center">
	<nav class="w-100">
		<div class="container-fluid d-flex justify-content-between align-items-center">
			{#if innerWidth > 1024}
				<div class="menu d-flex gap-3 w-50 justify-content-end pe-xl-5 pe-3">
					<!-- <div class="nav-item dropdown">
						<a class="nav-link dropdown-toggle " href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
							Products <i class="bi bi-chevron-down"></i>
						</a>
						<ul class="dropdown-menu  w-auto">
							<li><a class="dropdown-item " href="/products">Car Audio</a></li>
							<li><a class="dropdown-item " href="/products">Remote Start</a></li>
							<li><a class="dropdown-item " href="/products">Car Security</a></li>
							<li><a class="dropdown-item " href="/products">Dash Camera</a></li>
						</ul>
					</div>
					<a href="/our-services" class="txt-blanco ">Our services</a>
					<a href="/about" class="txt-blanco ">About us</a>
					<a href="/gallery" class="txt-blanco ">Gallery</a>
					<a href="/contact" class="txt-blanco ">Contact us</a> -->
				</div>
			{/if}
			

			<div class="logo">
				<a href="/" class="txt-blanco"><img src="../../images/logo-musicarro.png" alt=""></a>
			</div>

			<div class="menu d-flex gap-md-4 gap-2 justify-content-end align-items-center" class:w-50={innerWidth > 1024}>

				
				<!-- <div class="dropdown">
					<a class="d-flex dropdown-toggle " href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
						<div class="d-flex align-items-center gap-2 txt-blanco">
							{#if innerWidth > 768}
								<p>James Taylor</p>
							{/if}
							<div class="perfil rounded-circle fdo-rojo border border-white d-flex justify-content-center align-items-center">
								<div class="img-perfil fdo-gris-900 rounded-circle d-flex justify-content-center align-items-center">
									<h2 class="anton txt-24 text-center">JT</h2>
								</div>
							</div>
							<i class="bi bi-chevron-down"></i>
						</div>
					</a>
					<ul class="dropdown-menu">
						<li><a class="dropdown-item " href="#">Uno</a></li>
						<li><a class="dropdown-item " href="#">Dos</a></li>
						<li><a class="dropdown-item " href="#">Tres</a></li>
						<li><a class="dropdown-item " href="#">Cuatro</a></li>
					</ul>
				</div> -->
	
				<hr>
				<a href="#" class="btn btn-transparente d-flex align-items-center">
					<i class="bi bi-whatsapp me-md-2"></i>
						Boking Now
				</a>

				
					
				
			</div>
		</div>
	</nav>
</header>

<style>
	header {
		width: 100%;
		height: 60px;
		position: fixed;
		z-index: 2;
	}
	.logo img{
		height: 60px;
	}
	hr{
		width: 1px;
		height: 60px;
		background-color: var(--color-blanco);
		opacity: 1;
	}
	.perfil{
		width: 45px;
		height: 45px;
	}
	.img-perfil{
		width: 35px;
		height: 35px;
	}
	.dropdown-toggle::after {
		display: none;
	}
	.dropdown-menu{
		width: 185px;
	}
	@media screen and (max-width: 1200px){
		.menu a{
			font-size: var(--txt-14);
		}
		header {
			height: 50px;
		}
		hr{
			height: 50px;
		}
		.logo img{
			height: 50px;
		}
		.perfil{
			width: 40px;
			height: 40px;
		}
		.img-perfil{
			width: 30px;
			height: 30px;
		}
		.perfil h2{
			font-size: var(--txt-18);
		}
	}
	@media screen and (max-width: 1024px){
		.container-fluid{
			padding-left: 0px;
		}
	}
	@media screen and (max-width: 768px){
		/* .btn-transparente{
			font-size: var(--txt-20) !important;
			padding: 0px;
			width: 40px;
			height: 40px;
			border: none;
			text-align: center;
			justify-content: center;
		}
		hr{
			display: none;
		} */
		 .bi{
			display: none;
		 }
		 .btn-transparente{
			width: 150px;
			margin-right: 0px;
		 }
	}

	
</style>
