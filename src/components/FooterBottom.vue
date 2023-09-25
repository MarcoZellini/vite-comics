<script>
import AppButton from './AppButton.vue'

export default {
    name: "FooterBottom",
    components: {
        AppButton
    }
}
</script>

<template>
    <section id="others" class="py-5">
        <div class="container d-flex justify-content-between align-items-center">
            <!-- Bottone signup -->
            <AppButton />

            <!-- Lista di social -->
            <ul class="social d-flex align-items-center m-0">
                <a class="nav-item nav-link mx-1" href="#">Follow us</a>
                <a class="nav-item nav-link mx-1" href="#">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a>
                <a class="nav-item nav-link mx-1" href="#">
                    <img src="../assets/img/footer-twitter.png" alt="">
                </a>
                <a class="nav-item nav-link mx-1" href="#">
                    <img src="../assets/img/footer-youtube.png" alt="">
                </a>
                <a class="nav-item nav-link mx-1" href="#">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                </a>
                <a class="nav-item nav-link mx-1" href="#">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </a>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#others {
    background-color: $dc_dark_soft;
    position: relative;
    z-index: 10;
    color: $dc_light;

    .social {
        color: $dc_primary;
        text-transform: uppercase;
    }
}
</style>