<script>
export default {
    name: "PageMain",
}
</script>

<template>
    <!-- prima sezione -->
    <section class="one">
        <div class="container">
            <div class="row justify-content-center">
                <!-- titoli e sottotitoli -->
                <div class="col-12 col-lg-7 d-flex flex-column">
                    <h5 class="title_ text-center fw-light ">Our Love For Animation</h5>
                    <h2 class="title_ text-center fs-1 fw-bold purple_">We're Storytelling Experts With Creative
                        Smarts</h2>
                    <p class="title_ text-center fw-lighter purple_">
                        Our culture inspires the creative and innovative spirit found throughout our Studio. We
                        breathe life new ideas!
                    </p>
                </div>
                <!-- card -->
                <div class="col-12  d-flex gap-2 flex-wrap justify-content-center">
                    <div class="col-12 col-lg-3 border rounded-5 p-3 text-center">
                        <img src="../assets/img/smart1.png" alt="smart-1">
                        <h3 class="purple_">3D modeling</h3>
                        <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                            the results you
                            crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                    </div>
                    <div class="col-12 col-lg-3 border rounded-5 p-3 text-center">
                        <img src="../assets/img/smart2.png" alt="smart-2">
                        <h3 class="purple_">Collaboration</h3>
                        <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                            the results you
                            crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                    </div>
                    <div class="col-12 col-lg-3 border rounded-5 p-3 text-center">
                        <img src="../assets/img/smart3.png" alt="smart-3">
                        <h3 class="purple_">Creativity</h3>
                        <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                            the results you
                            crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                    </div>
                </div>
                <div class="col-12 d-flex flex-row-reverse d-none d-md-none d-lg-flex">
                    <img class="rocket" src="../assets/img/smart4.png" alt="smart-4">
                </div>
            </div>
        </div>
    </section>

    <!-- seconda sezione -->
    <section class="two">
        <img src="../assets/img/shape-top.png" alt="shape-top">
        <div class="container-fluid text-center p-5">
            <h2 class="text-white fs-1">Anidio Quick Facts</h2>
            <div class="row gap-4 justify-content-center">
                <div class="col-lg-2 border rounded-3 d-flex flex-wrap align-items-center justify-content-center p-4">
                    <h2 class="fw-bolder fs-1 text-white">700+</h2>
                    <small class="orange_">Projects done</small>
                </div>
                <div
                    class="col-12 col-lg-2 border rounded-3 d-flex flex-wrap align-items-center justify-content-center p-4">
                    <h2 class="fw-bolder fs-1 text-white">250+</h2>
                    <small class="orange_">Happy Clients</small>
                </div>
                <div
                    class="col-12 col-lg-2 border rounded-3 d-flex flex-wrap align-items-center justify-content-center p-4">
                    <h2 class="fw-bolder fs-1 text-white">25+</h2>
                    <small class="orange_">Team Members</small>
                </div>
                <div
                    class="col-12 col-lg-2 border rounded-3 d-flex flex-wrap align-items-center justify-content-center p-4">
                    <h2 class="fw-bolder fs-1 text-white">12+</h2>
                    <small class="orange_">Yearsn on the market</small>
                </div>
            </div>
        </div>
        <img src="../assets/img/shape-bottom.png" alt="shape-bottom">
    </section>

    <!-- terza sezione -->
    <section></section>

    <!-- quarta sezione -->
    <section></section>

    <!-- quinta sezione -->
    <section></section>

    <!-- sesta sezione -->
    <section></section>

    <!-- settima sezione -->
    <section></section>
</template>

<style scoped lang="scss">
@use '../style/general.scss' as *;

.orange_ {
    color: $orange;
}

.one {
    background-image: url(../assets/img/smart.png);
    background-repeat: no-repeat;
    background-size: contain;
    background-position: -10%;

    .col-4 {
        img {
            width: 100%;
        }
    }

    .purple_ {
        color: $purple;
    }

    h5 {
        color: mediumpurple;
    }

    .card {
        img {
            width: 50%;
        }
    }

    .rocket {
        width: 15%;
        height: 75%;
    }
}

.two {
    background-image: url(../assets/img/counter-bg.png);
    background-repeat: no-repeat;
    background-size: cover;

    img {
        width: 100%;
        display: block
    }

    .container-fluid {
        background-image: url(../assets/img/globe1.png);
        background-repeat: no-repeat;
        background-size: contain;
        background-position: 50%;
    }
}
</style>