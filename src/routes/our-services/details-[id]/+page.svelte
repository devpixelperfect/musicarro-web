<script>
    import Banner from "$lib/components/banners/Banner.svelte";
    import Marcas from "$lib/components/carrusel/Marcas.svelte";
    import Productos from "$lib/components/carrusel/Productos.svelte";
</script>

<!-- Banner component -->
<Banner texto="Our Services" imagen="service-details"/>

<section class="fdo-blanco-50 py-5">
    <div class="container">
        <form>
            <div class="row">
                <div class="col-12 col-md-6">
                    <h2 class="anton mb-3">Select a Date and Time</h2>
                    <p class="mb-4">Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam.</p>
                    <div class="row mb-3 mb-md-4">
                        <div class="col-12">
                            <label for="preferences" class="form-label">Preferences</label>
                            <div class="input-group">
                                <span class="input-group-text fw-bolder" id="icon-parent">
                                    <i class="bi bi-person"></i>
                                </span>
                                <select id="preferences" class="form-select" ria-describedby="icon-parent">
                                    <option selected>Open this select menu</option>
                                    <option value="1">1</option>
                                    <option value="2">2</option>
                                    <option value="3">3</option>
                                </select>
                            </div>
                        </div>
                    </div>
                    <div class="row mb-3 mb-md-0">
                        <div class="col-12 col-md-6 mb-3">
                            <label for="date" class="form-label">Date</label>
                            <input type="date" id="date" class="form-control">
                        </div>
                        <div class="col-12 col-md-6 mb-3">
                            <label for="time" class="form-label">Time</label>
                            <input type="time" id="time" class="form-control">
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-6">
                    <h2 class="anton mb-3">Services Details</h2>
                    <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam.</p>
                    <p class="mb-4">Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus</p>
                    <button class="btn btn-rojo">
                        Book appointment
                        <i class="bi bi-bookmark ms-2"></i>
                    </button>
                </div>
            </div>
        </form>
    </div>
</section>

<!-- Secciones adicionales -->
<Marcas/>
<Productos/>

<style>
    .form-select, select {
        border-left: none !important;
    }

    @media only screen and (max-width: 768px) {
        button {
            width: 100%;
        }
    }
</style>