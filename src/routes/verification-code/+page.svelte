<section class="fdo-blanco-50 py-5">
    <div class="container">
        <div class="d-flex flex-column align-items-center text-center">
            <div class="mb-5">
                <h2 class="anton mb-3">We need to verify your account</h2>
                <p>Each purchase is protected and it is necessary to verify your user account for security.</p>
            </div>
            <div class="fdo-blanco p-4 p-md-5">
                <div class="d-flex flex-column align-items-center gap-3">
                    <div class="d-flex flex-column align-items-center">
                        <h3 class="anton txt-40 lg-txt-32 mb-2">Code sent</h3>
                        <p class="numero">We send a verification code to your phone number <span class="fw-bold">xx xxx xxx89</span></p>
                    </div>
                    
                    <p class="fw-bold">Please enter the code here</p>
                </div>
                <div class="code-input d-flex justify-content-between mt-4 mb-4 mb-md-5">
                    <input type="text" maxlength="1" class="fw-bold txt-40">
                    <input type="text" maxlength="1" class="fw-bold txt-40">
                    <input type="text" maxlength="1" class="fw-bold txt-40">
                    <input type="text" maxlength="1" class="fw-bold txt-40">
                </div>
                <div class="d-flex flex-column flex-md-row justify-content-between gap-3 gap-md-0">
                    <div class="text-start">
                        <p class="">Didn't receive the code?</p>
                        <a href="" class="color-rojo fw-bold">Send code again</a>
                    </div>
                    <button class="btn btn-negro">
                        Check code
                        <i class="bi bi-check ms-2"></i>
                    </button>
                </div>
            </div>
        </div>
    </div>
</section>

<style>
    .fdo-blanco {
        max-width: 600px;
    }

    .numero {
        width: 70%;
    }

    .code-input input {
        width: 100px;
        height: 100px !important;
        text-align: center;
        font-size: var(--txt-40) !important;
    }

    input:focus {
	    border-color: var(--color-rojo) !important;
        background-color: var(--color-rojo);
        color: var(--color-blanco) !important;
    }

    a {
        color: var(--color-rojo);
    }

    @media only screen and (max-width: 768px) {
        .code-input input {
            width: 80px;
            height: 80px !important;
        }
    }

    @media only screen and (max-width: 576PX) {
        .code-input input {
            width: 60px;
            height: 60px !important;
        }

        .numero {
            width: 100%;
        }
    }
</style>