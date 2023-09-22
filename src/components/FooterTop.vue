<script>
export default {
    name: 'FooterTop'
}
</script>

<template>
    <section id="useful_links">
        <div class="container py-5">
            <div class="row justify-content-between">
                <div class="col-7">
                    <div class="row">
                        <div class="col-4 text-light">
                            <h5 class="text-uppercase">Dc Comics</h5>
                            <ul class="list-unstyled">
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                            <h5 class="text-uppercase">Shop</h5>
                            <ul class="list-unstyled">
                                <li>Shop Dc</li>
                                <li>Shop Dc Collectibles</li>
                            </ul>
                        </div>
                        <!-- /.col -->
                        <div class="col-4 text-light">
                            <h5 class="text-uppercase">Dc</h5>
                            <ul class="list-unstyled">
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                                <li>News</li>
                            </ul>
                        </div>
                        <!-- /.col -->
                        <div class="col-4 text-light">
                            <h5 class="text-uppercase">Sites</h5>
                            <ul class="list-unstyled">
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                        </div>
                        <!-- /.col -->
                    </div>
                </div>
                <!-- /.col-6 -->
                <div class="col-5 position-relative d-flex justify-content-center align-items-center">
                    <img class="dc_logo img-fluid" src="..\assets\img\dc-logo-bg.png" alt="">
                </div>
                <!-- /.col-6 -->
            </div>
            <!-- /.row -->

        </div>
        <!-- /.container -->
    </section>
    <!-- /#useful_links -->
</template>

<style>
#useful_links {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.dc_logo {
    position: absolute;
    /* top: 0; */
    /* right: 50; */
    /* z-index: 0; */
    /* margin-top: -1rem; */
}
</style>