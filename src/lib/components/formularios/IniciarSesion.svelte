<div class="formulario fdo-blanco px-sm-4 py-5">
    <div class="d-flex justify-content-end">
        <a href="/" class="txt-14 link-negro semi-bold"><i class="bi bi-arrow-left-circle-fill me-3"></i> Back to home</a>
    </div>
    <h2 class="anton text-center mt-3">Welcome</h2>
    <p class="text-center px-3 mt-3">Lorem ipsum dolor sit amet consectetur adipiscing eli mattis sit phasellus mollis sit aliquam sit nullam.</p>
    <form>
        <div class="mb-3 mt-4">
            <label for="exampleFormControlInput1" class="form-label">Email</label>
            <div class="position-relative">
                <input type="email" class="form-control ps-5" id="exampleFormControlInput1" placeholder="name@example.com">
                <i class="bi bi-envelope txt-20"></i>
            </div>
            
        </div>
        <div class="mb-3">
            <label for="exampleFormControlInput1" class="form-label">Pasword</label>
            <div class="position-relative">
                
                <input type="password" class="form-control px-5" id="exampleFormControlInput1" placeholder="***********">
                <i class="bi bi-lock txt-20"></i>
                <i class="bi bi-eye txt-20"></i>
            </div>
            
        </div>
        <div class="d-flex justify-content-end">
            <a href="/account/reset" class="txt-14 link-rojo">Forgot your password?</a>
        </div>
        <button type="submit" class="btn btn-rojo w-100 mt-4 d-flex align-items-center justify-content-center">Sign in <i class="bi bi-box-arrow-in-right ms-2 "></i></button>
    </form>
    <hr class="my-4">
    <div class="d-flex justify-content-center">
        <p class="txt-14">Are you new? <a href="/account/create" class="link-rojo txt-14">Created an Account</a></p>
    </div>
</div>

<style>
    .formulario{
        width: 100%;
        max-width: 450px;
    }

    .position-relative i{
        position: absolute;
        left: 15px;
        top: 10px;
    }
    .position-relative .bi-eye {
        right: 15px !important;
        left: inherit;
        cursor: pointer;
    }

</style>