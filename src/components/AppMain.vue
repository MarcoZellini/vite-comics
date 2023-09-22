<script>
export default {
    name: 'AppMain'
}
</script>

<template>
    <main id="app_main">

        <section id="content">
            <div class="container">
                <h6 class="py-5">--&gt; Content goes here &lt;--</h6>
            </div>
            <!-- /.container -->
        </section>
        <!-- /#content -->

        <section id="main_menu">
            <div class="container">
                <ul class="list-unstyled d-flex justify-content-around align-items-center py-5 m-0">
                    <li class="d-flex align-items-center p-3">
                        <a href="#" class="d-flex align-items-center">
                            <div class="item_img">
                                <img class="img-fluid" src="../assets/img/buy-comics-digital-comics.png" alt="">
                            </div>
                            <span>Digital Comics</span>
                        </a>
                    </li>
                    <li class="d-flex align-items-center p-3">
                        <a href="#" class="d-flex align-items-center">
                            <div class="item_img">
                                <img class="img-fluid" src="../assets/img/buy-comics-merchandise.png" alt="">
                            </div>
                            <span>DC Merchandise</span>
                        </a>
                    </li>
                    <li class="d-flex align-items-center p-3">
                        <a href="#" class="d-flex align-items-center">
                            <div class="item_img">
                                <img class="img-fluid" src="../assets/img/buy-comics-subscriptions.png" alt="">
                            </div>
                            <span>Subscription</span>
                        </a>
                    </li>
                    <li class="d-flex align-items-center p-3">
                        <a href="#" class="d-flex align-items-center">
                            <div class="item_img">
                                <img class="img-fluid" src="../assets/img/buy-comics-shop-locator.png" alt="">
                            </div>
                            <span>Comic Shop Locator</span>
                        </a>
                    </li>
                    <li class="d-flex align-items-center p-3">
                        <a href="#" class="d-flex align-items-center">
                            <div class="item_img">
                                <img class="img-fluid visa_card" src="../assets/img/buy-dc-power-visa.svg" alt="">
                            </div>
                            <span>DC Power Visa</span>
                        </a>
                    </li>


                </ul>
            </div>
            <!-- /.container -->
        </section>
        <!-- /#main_menu -->

    </main>
    <!-- /#app_main -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#app_main {
    position: relative;
    z-index: 10;

    #content {
        background-color: $dc_dark;
        color: $dc_light;

        h6 {
            margin: 0;
        }
    }

    #main_menu {
        background-color: $dc_primary;

        li>a {
            color: $dc_light;
            text-decoration: none;
            text-transform: uppercase;

            .item_img img {
                max-height: 60px;
                margin-right: 1rem;
            }
        }
    }
}

.visa_card {
    height: 50px;
}
</style>