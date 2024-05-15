<script>
    import Banner from "$lib/components/banners/Banner.svelte";
</script>

<!-- Banner component -->
<Banner texto="Contact Us" imagen="contact-us"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <div class="row">
            <div class="col-12 col-md-6">
                <h2 class="anton mb-3">Contact us we are ready to respond</h2>
                <p class="mb-4">Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam.</p>
                
                <form>
                    <div class="row mb-3">
                        <div class="col-12">
                            <label for="nombre" class="form-label">Full name</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-person"></i>
                                </span>
                                <input type="text" id="nombre" class="form-control">
                            </div>
                        </div>
                    </div>

                    <div class="row mb-3">
                        <div class="col-12 col-md-6 mb-3 mb-md-0">
                            <label for="mail" class="form-label">Email</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-envelope"></i>
                                </span>
                                <input type="email" id="mail" class="form-control">
                            </div>
                        </div>
                        <div class="col-12 col-md-6">
                            <label for="telefono" class="form-label">Phone</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder pe-1">
                                    <i class="bi bi-telephone"></i>
                                </span>
                                <input type="phone" id="telefono" class="form-control">
                            </div>
                        </div>
                    </div>

                    <div class="row mb-3">
                        <div class="col-12">
                            <label for="mensaje" class="form-label">Message</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder d-flex align-items-start pt-2 pe-1">
                                    <i class="bi bi-chat-left"></i>
                                </span>
                                <textarea class="form-control" id="mensaje" rows="3"></textarea>
                            </div>
                        </div>
                    </div>

                    <div class="d-flex justify-content-end">
                        <button class="btn btn-rojo">
                            Send message
                            <i class="bi bi-send ms-2"></i>
                        </button>
                    </div>
                </form>
            </div>

            <div class="mapa col-12 col-md-6 mt-5 mt-md-0">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2931.313896232727!2d-71.18127982363464!3d42.7182464711619!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89e3079ddb9e3c3f%3A0x35818ee5819920fd!2sMusicarro%20Auto%20Sound!5e0!3m2!1ses!2smx!4v1715093476009!5m2!1ses!2smx" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </div>
    </div>
</section>

<style>
    input, textarea {
        border-left: none !important;
    }

    @media only screen and (max-width: 768px) {
        button {
            width: 100%;
        }

        .mapa {
            height: 500px;
        }
    }
</style>