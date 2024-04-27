<script>
	
</script>

<header class="fdo-rojo txt-blanco d-flex align-items-center">
	<nav class="w-100">
		<div class="container-fluid d-flex justify-content-between align-items-center">
			<div class="menu d-flex gap-3 w-50 justify-content-end pe-5">
				<div class="nav-item dropdown">
					<a class="nav-link dropdown-toggle txt-16" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
						Products <i class="bi bi-chevron-down"></i>
					</a>
					<ul class="dropdown-menu  w-auto">
						<li><a class="dropdown-item txt-16" href="#">Car Audio</a></li>
						<li><a class="dropdown-item txt-16" href="#">Remote Start</a></li>
						<li><a class="dropdown-item txt-16" href="#">Car Security</a></li>
						<li><a class="dropdown-item txt-16" href="#">Dash Camera</a></li>
					</ul>
				</div>
				<a href="/nosotros" class="txt-blanco txt-16">Our services</a>
				<a href="/contacto" class="txt-blanco txt-16">About us</a>
				<a href="/contacto" class="txt-blanco txt-16">Gallery</a>
				<a href="/contacto" class="txt-blanco txt-16">Contact us</a>
			</div>

			<div class="logo">
				<a href="/" class="txt-blanco"><img src="../../images/logo-musicarro.png" alt=""></a>
			</div>

			<div class="menu d-flex w-50 gap-4 justify-content-end align-items-center">

				
				<div class="dropdown">
					<a class="d-flex dropdown-toggle txt-16" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
						<div class="d-flex align-items-center gap-2 txt-blanco">
							<p class="txt-16">James Taylor</p>
							<div class="perfil rounded-circle fdo-rojo border border-white d-flex justify-content-center align-items-center">
								<div class="img-perfil fdo-gris-900 rounded-circle d-flex justify-content-center align-items-center">
									<h2 class="anton txt-24 text-center">JT</h2>
								</div>
							</div>
							<i class="bi bi-chevron-down"></i>
						</div>
					</a>
					<ul class="dropdown-menu">
						<li><a class="dropdown-item txt-16" href="#">Uno</a></li>
						<li><a class="dropdown-item txt-16" href="#">Dos</a></li>
						<li><a class="dropdown-item txt-16" href="#">Tres</a></li>
						<li><a class="dropdown-item txt-16" href="#">Cuatro</a></li>
					</ul>
				</div>
	
				<hr>
				<a href="/contacto" class="btn btn-transparente d-flex align-items-center"><i class="bi bi-cart2 me-2"></i> Cart</a>
			</div>
		</div>
	</nav>
</header>

<style>
	header {
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
</style>
