<script>
export default {
    name: "PageMain",
    data() {
        return {
            currentCard: 0,
        }
    },
    methods: {
        changeCardBack() {
            this.currentCard--;
            if (this.currentCard < 0) {
                this.currentCard = 3;
            }
            return this.currentCard;
        },
        changeCardNext() {
            this.currentCard++;
            if (this.currentCard >= 4) {
                this.currentCard = 0;
            }
            return this.currentCard;
        }
    },
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
                    <div id="bg_orange_gradient" class="col-12 col-lg-3 border rounded-5 p-3 text-center">
                        <img src="../assets/img/smart1.png" alt="smart-1">
                        <h3 class="purple_ my-3">3D modeling</h3>
                        <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                            the results you
                            crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                    </div>
                    <div id="bg_purple_gradient" class="col-12 col-lg-3 border rounded-5 p-3 text-center">
                        <img src="../assets/img/smart2.png" alt="smart-2">
                        <h3 class="purple_ my-3">Collaboration</h3>
                        <p class="fw-lighter">We constantly ask questions. It helps us shape your story and deliver
                            the results you
                            crave. Yep, we'Il drill deep to deliver above and beyond yout expectacions.</p>
                    </div>
                    <div id="bg_pink_gradient" class="col-12 col-lg-3 border rounded-5 p-3 text-center">
                        <img src="../assets/img/smart3.png" alt="smart-3">
                        <h3 class="purple_ my-3">Creativity</h3>
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
    <section class="three my-5">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-6 text-center">
                    <h6 class="fw-light">Our Works</h6>
                    <h2 class="fw-bolder purple_">Featured Productions</h2>
                    <p class="fw-lighter">
                        Here's just small of some of those projects that we're quite proud of. If you're
                        looking for something specific feel free to get in contact with us
                    </p>
                </div>
            </div>
        </div>
        <div class="container my-3">
            <div class="row gap-2 justify-content-center">
                <div class="col-5 rounded-3">
                    <img src="../assets/img/work1.png" alt="work-1">
                </div>
                <div class="col-5 rounded-3">
                    <img src="../assets/img/work2.png" alt="work-2">
                </div>
                <div class="col-5 rounded-3">
                    <img src="../assets/img/work3.png" alt="work-3">
                </div>
                <div class="col-5 rounded-3">
                    <img src="../assets/img/work4.png" alt="work-4">
                </div>
                <div class="col-3 text-center my-3">
                    <button class="border-1 border-light bg-white purple_ px-3 py-1 rounded-5">
                        See Our Work
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- quarta sezione -->
    <section class="four">
        <div class="container-fluid">
            <div class="row">
                <div class="col-6">
                    <img class="thumb_" src="../assets/img/process-thumb.png" alt="process-thumb">
                </div>
                <div class="col-6">
                    <div class="row gap-2">
                        <div class="col-8">
                            <h5>Our Process</h5>
                            <h2 class="fs-1 fw-bold purple_">Our Process for Your Animation Production</h2>
                            <p class="fw-lighter">We have an effective process for working on animation</p>
                        </div>
                        <div v-if="currentCard == 0"
                            class="col-5 text-center border rounded-5 p-4 flex-column align-items-center">
                            <div class="img_ p-3 rounded-circle">
                                <img src="src/assets/img/process2.png" alt="process-2">
                                <div class="number_ p-2 d-flex align-items-end text-black-50 rounded-bottom">
                                    <small>1</small>
                                </div>
                            </div>
                            <h3 class="purple_ my-3">Pre-Production</h3>
                            <p class="fw-lighter">
                                We'll take your idea and create a technical script which consists of action notes and
                                animation descriptions.
                            </p>
                        </div>
                        <div v-else-if="currentCard == 1"
                            class="col-5 text-center border rounded-5 p-4 flex-column align-items-center">
                            <div class="img_ p-3 rounded-circle">
                                <img src="src/assets/img/process1.png" alt="process-1">
                                <div class="number_ p-2 d-flex align-items-end text-black-50 rounded-bottom">
                                    <small>2</small>
                                </div>
                            </div>
                            <h3 class="purple_ my-3">Pre-Production</h3>
                            <p class="fw-lighter">
                                We'll take your idea and create a technical script which consists of action notes and
                                animation descriptions.
                            </p>
                        </div>
                        <div v-else-if="currentCard == 2"
                            class="col-5 text-center border rounded-5 p-4 flex-column align-items-center">
                            <div class="img_ p-3 rounded-circle">
                                <img src="src/assets/img/process2.png" alt="process-2">
                                <div class="number_ p-2 d-flex align-items-end text-black-50 rounded-bottom">
                                    <small>3</small>
                                </div>
                            </div>
                            <h3 class="purple_ my-3">Pre-Production</h3>
                            <p class="fw-lighter">
                                We'll take your idea and create a technical script which consists of action notes and
                                animation descriptions.
                            </p>
                        </div>
                        <div v-else-if="currentCard == 3"
                            class="col-5 text-center border rounded-5 p-4 flex-column align-items-center">
                            <div class="img_ p-3 rounded-circle">
                                <img src="src/assets/img/process1.png" alt="process-1">
                                <div class="number_ p-2 d-flex align-items-end text-black-50 rounded-bottom">
                                    <small>4</small>
                                </div>
                            </div>
                            <h3 class="purple_ my-3">Pre-Production</h3>
                            <p class="fw-lighter">
                                We'll take your idea and create a technical script which consists of action notes and
                                animation descriptions.
                            </p>
                        </div>
                        <div class="col-12 d-flex">
                            <div @click="changeCardBack"
                                class="arrow_ p-3 border rounded-circle d-flex align-items-center justify-content-center m-1 text-black-50">
                                <font-awesome-icon icon="fa-solid fa-arrow-left" />
                            </div>
                            <div @click="changeCardNext"
                                class="arrow_ p-3 border rounded-circle d-flex align-items-center justify-content-center m-1 text-black-50">
                                <font-awesome-icon icon="fa-solid fa-arrow-right" />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

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

.purple_ {
    color: $purple;
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

    .col-12 {
        #bg_orange_gradient {
            background: rgb(255, 183, 134);
            background: linear-gradient(0deg, rgba(255, 183, 134, 1) 0%, rgba(255, 255, 255, 1) 100%);
        }

        #bg_purple_gradient {
            background: rgb(174, 147, 210);
            background: linear-gradient(0deg, rgba(174, 147, 210, 1) 0%, rgba(255, 255, 255, 1) 100%);
        }

        #bg_pink_gradient {
            background: rgb(255, 222, 255);
            background: linear-gradient(0deg, rgba(255, 222, 255, 1) 0%, rgba(255, 255, 255, 1) 100%);
        }
    }

    .purple_ {
        color: $purple;
    }

    h5 {
        color: $violet;
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

.three {
    .col-6 {
        h6 {
            color: $violet;
        }
    }

    .col-5 {
        img {
            width: 100%;
        }
    }
}

.four {
    .col-6 {
        position: relative;

        .thumb_ {
            width: 100%;
            position: absolute;
            left: -190px;
        }
    }

    .col-5 {
        position: relative;
        display: flex;

        .img_ {
            width: 80px;
            height: 80px;
            background-color: #fff9f5;

            img {
                object-fit: contain;
                width: 100%;
                height: 100%;
            }

            .number_ {
                height: 20%;
                background-color: $light_violet;
                position: absolute;
                top: 0;
                right: 12%;
            }
        }
    }
}
</style>

