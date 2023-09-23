<script>
import FooterLinks from './FooterLinks.vue'

export default {
    name: 'FooterTop',
    components: {
        FooterLinks
    }
}
</script>

<template>
    <div id="footer_top">
        <div class="container py-5">
            <div class="row align-items-center">
                <div class="col-7">
                    <FooterLinks />
                </div>
                <!-- /.col-7 -->
                <div class="col-5">
                    <div class="position-relative d-flex justify-content-center align-items-center">
                        <img class="img-fluid position-absolute" src="..\assets\img\dc-logo-bg.png" alt="">
                    </div>
                </div>
                <!-- /.col-5 -->
            </div>
        </div>
    </div>
</template>

<style>
#footer_top {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    z-index: 0;
}
</style>