<script>
    import Titulo from "$lib/components/utilidades/Titulo.svelte";
	import CardHistorial from "$lib/components/account/Card-historial.svelte";

    let imagenCargada = '';
    let icono = 'bi bi-person txt-rojo txt-100';

    function cambiarFoto(e) {
        const file = e.target.files[0];
        if (file) {
            const reader = new FileReader();
            reader.onload = () => {
                imagenCargada = reader.result;
            };
            reader.readAsDataURL(file);
        } else {
            imagenCargada = '';
        }
    }
</script>

<div class="fdo-blanco">
    <div class="container pt-4">
        <Titulo titulo="Account Settings"/>
    </div>
</div>

<section class="fdo-blanco-50 py-3 py-md-5">
    <div class="container">
        <div class="row">
            <div class="col-12 col-lg-6">
                <div class="perfil p-5">

                    <div class="d-flex align-items-center justify-content-center mb-5">
                        <div class="position-relative icono-usuario-border d-flex justify-content-center align-items-center">
                            <div class="icono-usuario d-flex align-items-center justify-content-center">
                                {#if imagenCargada}
                                    <img src={imagenCargada} alt="foto de usuario" class="foto-usuario"/>
                                {:else}
                                    <i class={icono}></i>
                                {/if}
                            </div>
                            <div class="icono-camara position-absolute bottom-0 end-0 fdo-gris-50 d-flex align-items-center justify-content-center">
                                <input type="file" accept="image/*" id="fileInput" on:change={cambiarFoto}/>
                                <label for="fileInput" class="camera-icon">
                                    <i class="bi bi-camera txt-24"></i>
                                </label>
                            </div>
                        </div>
                    </div>

                    <div class="row mb-3">
                        <div class="col-12">
                            <label for="nombre" class="form-label txt-blanco">Full name</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-person"></i>
                                </span>
                                <input type="text" id="nombre" class="form-control">
                            </div>
                        </div>
                    </div>

                    <div class="row mb-3">
                        <div class="col-12">
                            <label for="mail" class="form-label txt-blanco">Email</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-envelope"></i>
                                </span>
                                <input type="email" id="mail" class="form-control">
                            </div>
                        </div>
                    </div>

                    <div class="row mb-3">
                        <div class="col-12">
                            <label for="password" class="form-label txt-blanco">Password</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-lock"></i>
                                </span>

                                <input type="password" id="password" class="form-control">

                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-eye"></i>   
                                </span>
                            </div>
                        </div>
                    </div>

                    <div class="linea my-4"></div>

                    <div class="mb-3">
                        <a href="" class="txt-blanco">
                            <i class="bi bi-box-arrow-right me-2"></i>
                            Sign out
                        </a>
                    </div>

                    <div class="d-flex justify-content-end">
                        <a href="" class="txt-rojo eliminar">
                            <i class="bi bi-trash me-2"></i>
                            Delete my account
                        </a>
                    </div>

                </div>

            </div>

            <div class="col-12 col-lg-6 my-4 my-lg-0">
                <h3 class="anton mb-3 text-md-end">Shopping history</h3>
                <div class="historial">
                    <CardHistorial titulo="Music set up installation" descripcion="Lorem ipsum dolor sit amet conse bolli tetur adipiscing elit tortor eu."/>
                    <CardHistorial titulo="Music set up installation" descripcion="Lorem ipsum dolor sit amet conse bolli tetur adipiscing elit tortor eu."/>
                    <CardHistorial titulo="Music set up installation" descripcion="Lorem ipsum dolor sit amet conse bolli tetur adipiscing elit tortor eu."/>
                    <CardHistorial titulo="Music set up installation" descripcion="Lorem ipsum dolor sit amet conse bolli tetur adipiscing elit tortor eu."/>
                    <CardHistorial titulo="Music set up installation" descripcion="Lorem ipsum dolor sit amet conse bolli tetur adipiscing elit tortor eu."/>
                    <CardHistorial titulo="Music set up installation" descripcion="Lorem ipsum dolor sit amet conse bolli tetur adipiscing elit tortor eu."/>
                </div>
            </div>
        </div>
    </div>
</section>

<style>
    .fdo-blanco {
        height: 90px;
    }

    .perfil {
        background: linear-gradient(220deg, var(--color-rojo) 10%, var(--color-gris-1000) 50%);
    }

    .icono-usuario-border {
        position: relative;
        width: 155px;
        height: 155px;
        border-radius: 50%;
        background: linear-gradient(135deg, var(--color-blanco) 10%, var(--color-rojo) 50%);
    }

    .icono-usuario {
        width: 150px;
        height: 150px;
        border-radius: 50%;
        background: radial-gradient(circle at center, var(--color-gris-800), var(--color-gris-1000));
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .foto-usuario {
        width: 100%;
        height: 100%;
        object-fit: cover;
        border-radius: 50%;
    }

    .icono-camara {
        width: 50px;
        height: 50px;
        border-radius: 50%;
    }

    .camera-icon {
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
    }

    #fileInput {
        position: absolute;
        width: 100%;
        height: 100%;
        opacity: 0;
        cursor: pointer;
    }

    input {
        border-left: none !important;
    }

    input[type='password'] {
        border-right: none !important;
    }

    .linea {
        height: 0.5px;
        background-color: var(--color-blanco);
    }

    a:hover {
        color: var(--color-rojo) !important;
    }

    .eliminar:hover {
        color: var(--color-blanco) !important;
    }

    .historial {
        max-height: 630px;
        overflow-y: scroll;
    }

    @media only screen and (max-width: 768px) {
        .fdo-blanco {
            height: 75px;
        }
    }
</style>
