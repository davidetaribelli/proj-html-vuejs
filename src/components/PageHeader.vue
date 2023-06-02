<script>
export default {
    name: "PageHeader",
    props: [
        "linkArray",
    ],
}
</script>

<template>
    <!-- NavBar -->
    <section class="navSection">
        <div class="container">
            <div class="row">
                <div class="col-sm-12 col-md-11 mx-auto my-0 p-3 d-flex justify-content-around align-items-center">
                    <div class="logo_ p-3 d-flex justify-content-center align-items-center">
                        <img src="../assets/img/logo.png" alt="logo">
                    </div>
                    <div class="option_ p-3 d-flex justify-content-between align-items-center">
                        <nav class="navbar navbar-expand-lg">
                            <div class="container-fluid">
                                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup"
                                    aria-expanded="false" aria-label="Toggle navigation">
                                    <span class="navbar-toggler-icon"></span>
                                </button>
                                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                                    <div class="navbar-nav">
                                        <!-- utilizzo il v-for per stampare tutti gli elementi passati dall'array creato nell App -->
                                        <a v-for="link in linkArray" class="nav-link" href="#">
                                            {{ link.link }}
                                        </a>
                                        <button class="bg-white border-0 rounded-4 px-4">Get a Quote</button>
                                    </div>
                                </div>
                            </div>
                        </nav>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Title and jumbo-->
    <section class="jumboSection">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-sm-12 mx-auto my-0 d-flex flex-column align-items-center p-5">
                    <img class="globe_1 d-none d-md-none d-lg-block " src="../assets/img/globe1.png" alt="globe-1">
                    <h6 class="orange_">Imagine, Create, Experience</h6>
                    <h2 class="text-white">We Animate</h2>
                    <img class="globe_2  d-none d-md-none d-lg-block " src="../assets/img/globe2.png" alt="globe-2">
                    <img class="light_ d-none d-md-none d-lg-block " src="../assets/img/light.png" alt="light">
                    <h2 class="text-white my-3">With Ninja-Like Precision</h2>
                    <h6 class="text-white my-3">We are a character-driven animation studio striving to make high-quality
                        animations.</h6>
                    <img class="leftMan d-none d-md-none d-lg-block " src="../assets/img/left-man.png" alt="left-man">
                    <img class="rightMan d-none d-md-none d-lg-block " src="../assets/img/right-man.png" alt="right-man">
                </div>
                <div class="col-sm-12 col-md-4 text-center mb-5">
                    <button type="button" class="btn bg-white btn-sm mx-3 px-4 py-2 rounded-5">Start a Project</button>
                    <button type="button"
                        class="btn g-transparent btn-sm mx-3 px-3 py-2 rounded-5 text-white border">Portfolio</button>
                </div>
            </div>
        </div>
        <div class="container-fluid jumbo_container d-none d-lg-block">
            <div class="jumbo_ mx-auto my-0 rounded-5">
                <img src="../assets/img/middle.png" alt="middle">
                <div class="play_ d-flex align-items-center justify-content-center p-5 rounded-circle">
                    <font-awesome-icon class="fs-3 text-white" icon="fa-solid fa-play" />
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/general.scss' as *;

.navSection {
    .container {
        background-image: url(../assets/img/globe3.png);
        background-repeat: no-repeat;
        background-size: 20%;
        background-position: 45% 100%;

        .container-fluid {
            .navbar-nav {
                a {
                    color: white;

                    &:hover {
                        color: $orange;

                    }
                }
            }
        }


    }
}

.jumboSection {
    background-image: url(../assets/img/dots-left.png);
    background-repeat: no-repeat;
    background-position: contain;

    .container-fluid.jumbo_container {
        height: 300px;
        background-image: url(../assets/img/shape-bottom.png);
        background-size: contain;
        background-repeat: no-repeat;
        background-position: bottom;

        .jumbo_ {
            width: 1048px;
            height: 548px;
            position: relative;
            bottom: 15px;
            right: -6%;

            .play_ {
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                background-color: #a615ea;
            }
        }

    }

    .container {
        background-image: url(../assets/img/dots-right.png);
        background-repeat: no-repeat;
        background-position: right;
        background-size: contain;
        position: relative;

        .leftMan {
            height: 80%;
            position: absolute;
            left: -5%;
            bottom: 0;
        }

        .rightMan {
            height: 80%;
            position: absolute;
            right: -5%;
            bottom: 0;
        }

        .globe_1 {
            height: 27%;
            position: absolute;
            left: 8%;
            top: -7%;
        }

        .globe_2 {
            height: 20%;
            position: absolute;
            right: 31%;
            top: 20%;
        }

        .light_ {
            height: 20%;
            position: absolute;
            right: 12%;
            top: 0%;
        }

        h2 {
            font-size: 3.5rem;
            z-index: 1;
        }
    }
}

.logo_ {
    height: 100%;
}

button {
    color: $purple;

    &:hover {
        -webkit-box-shadow: 0px 10px 13px -7px #FFFFFF, 7px 0px 29px 0px rgba(255, 255, 255, 0.5);
        box-shadow: 0px 10px 13px -7px #FFFFFF, 7px 0px 29px 0px rgba(255, 255, 255, 0);
    }
}

h6.orange_ {
    color: $orange
}
</style>