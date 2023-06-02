<script>
export default {
    name: "PageFooter",
    props: [
        "arrayFooter",
    ],
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-12 border-bottom p-3">
                <div class="row justify-content-between align-items-center">
                    <div class="col-3">
                        <img src="../assets/img/footer-logo.png" alt="footer-logo">
                    </div>
                    <div class="col-7 d-flex justify-content-end">
                        <a v-for="link in arrayFooter" class="mx-3 text-decoration-none  text-black" href="#">
                            {{ link.link }}
                        </a>
                    </div>
                </div>
            </div>
            <div class="col-12 p-3">
                <div class="row justify-content-between align-items-center">
                    <div class="col-4">
                        <small class="fw-lighter">
                            Copyrigth © 2022
                            <a class="green_ text-decoration-none" href="#">Softivus.</a>
                            All rights reserved.
                        </small>
                    </div>
                    <div class="col-7 d-flex justify-content-end">
                        <div class="social_ d-flex justify-content-center gap-3 my-4">
                            <font-awesome-icon
                                class="icon_ p-2 border d-flex justify-content-center align-items-center rounded-circle green_"
                                icon="fa-brands fa-facebook-f" />
                            <font-awesome-icon
                                class="icon_ p-2 border d-flex justify-content-center align-items-center rounded-circle green_"
                                icon="fa-brands fa-twitter" />
                            <font-awesome-icon
                                class="icon_ p-2 border d-flex justify-content-center align-items-center rounded-circle green_"
                                icon="fa-brands fa-instagram" />
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <font-awesome-icon icon="fa-solid fa-arrow-up" class="p-3 border rounded-3 bg_purple text-white icon_arrow" />
    </div>
</template>

<style scoped lang="scss">
@use '../style/general.scss' as *;

.green_ {
    color: $green;
}

.bg_purple {
    background-color: $purple;
}

.container {
    position: relative;
}

.icon_ {
    width: 20px;
    height: 20px;
}

.icon_arrow {
    position: absolute;
    bottom: 5%;
    right: -5%;
}
</style>