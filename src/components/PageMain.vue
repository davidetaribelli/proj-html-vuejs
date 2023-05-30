<script>
export default {
    name: "PageMain",
}
</script>

<template>
    <!-- prima sezione -->
    <section>
        <div class="container">
            <div class="row">
                <div class="col-3">
                    immaginona
                </div>
                <div class="col-8">
                    <div class="row">
                        <div class="col-10 d-flex flex-column">
                            <h5 class="title_ text-center fw-light ">Our Love For Animation</h5>
                            <h2 class="title_ text-center fs-1 fw-bold purple_">We're Storytelling Experts With Creative
                                Smarts</h2>
                            <p class="title_ text-center fw-lighter purple_">
                                Our culture inspires the creative and innovative spirit found throughout our Studio. We
                                breathe life new ideas!
                            </p>
                        </div>
                        <div class="col-12 gap-2 d-flex">
                            <div class="col-4 border rounded-5 p-3 text-center">
                                <img src="../assets/img/smart1.png" alt="smart-1">
                                <h3 class="purple_">3D modeling</h3>
                                <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                                    the results you
                                    crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                            </div>
                            <div class="col-4 border rounded-5 p-3 text-center">
                                <img src="../assets/img/smart2.png" alt="smart-2">
                                <h3 class="purple_">Collaboration</h3>
                                <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                                    the results you
                                    crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                            </div>
                            <div class="col-4 border rounded-5 p-3 text-center">
                                <img src="../assets/img/smart3.png" alt="smart-3">
                                <h3 class="purple_">Creativity</h3>
                                <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                                    the results you
                                    crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                            </div>
                        </div>
                        <div class="col-12 d-flex flex-row-reverse">
                            <img class="rocket" src="../assets/img/smart4.png" alt="smart-4">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- seconda sezione -->
    <section></section>

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

.purple_ {
    color: $purple;
}

.title_ {
    width: 500px;
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
    position: relative;
    right: -120px;
}
</style>