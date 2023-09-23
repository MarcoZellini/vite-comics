<script>

export default {
    name: 'MainMenu',
    data() {
        return {
            menuItems: [
                {
                    url: '#',
                    imgPath: 'src/assets/img/buy-comics-digital-comics.png', /* Perche????  percorsi dell' immagine nello stesso punto ma devono essere scritti diversamente */
                    name: 'Digital Comics'
                },
                {
                    url: '#',
                    imgPath: 'src/assets/img/buy-comics-merchandise.png',
                    name: 'DC Merchandise'
                },
                {
                    url: '#',
                    imgPath: 'src/assets/img/buy-comics-subscriptions.png',
                    name: 'Subscription'
                },
                {
                    url: '#',
                    imgPath: 'src/assets/img/buy-comics-shop-locator.png',
                    name: 'Comic Shop Locator'
                },
                {
                    url: '#',
                    imgPath: 'src/assets/img/buy-dc-power-visa.svg',
                    name: 'DC Power Visa'
                },
            ]
        }
    }
}

</script>

<template>
    <section id="main_menu">
        <div class="container">
            <ul class="list-unstyled d-flex justify-content-around align-items-center py-5 m-0">


                <li v-for="item in menuItems" class="d-flex align-items-center p-3">
                    <a :href="item.url" class="d-flex align-items-center">
                        <div class="item_img">
                            <img class="img-fluid" :class="item.imgPath.includes('visa') ? 'visa_card' : ''"
                                :src="item.imgPath" alt="">
                        </div>
                        <span>{{ item.name }}</span>
                    </a>
                </li>

                <!-- Perche????  percorsi dell' immagine nello stesso punto ma devono essere scritti diversamente-->

                <!-- <li class="d-flex align-items-center p-3">
                    <a href="#" class="d-flex align-items-center">
                        <div class="item_img">
                            <img class="img-fluid" src="../assets/img/buy-comics-merchandise.png" alt="">
                        </div>
                        <span>DC Merchandise</span>
                    </a>
                </li> -->

            </ul>
        </div>
        <!-- /.container -->
    </section>
    <!-- /#main_menu -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

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

.visa_card {
    height: 50px;
}
</style>