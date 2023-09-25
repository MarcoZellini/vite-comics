<script>
import AppHero from './AppHero.vue'
import MainMenu from './MainMenu.vue'
import AppProduct from './AppProduct.vue'
import products from '../products'

export default {
    name: 'AppMain',
    components: {
        MainMenu,
        AppHero,
        AppProduct
    },
    data() {
        return {
            products
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    },

}
</script>

<template>
    <main id="app_main">
        <AppHero :imgPath="getImageUrl('jumbotron.jpg')" />

        <section id="product_list" class="container">

            <div class="container">
                <div class="title">current series</div>
            </div>

            <div class="row px-3">
                <div class="col-2" v-for="item in products">
                    <AppProduct :href="item.thumb" :title="item.series" />
                </div>
            </div>

            <div class="more d-flex justify-content-center align-items-center pt-3">
                <a class="btn btn-primary rounded-0 text-light text-uppercase">load more</a>
            </div>

        </section>
        <!-- /#product_list -->

        <MainMenu />

    </main>
    <!-- /#app_main -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#app_main {
    position: relative;
    z-index: 10;
    background-color: $dc_dark;

    #product_list.container {
        padding-top: 4rem;
        padding-bottom: 2rem;
        position: relative;

        .title {
            background-color: $dc_primary;
            font-size: 1.5rem;
            height: 55px;
            width: 250px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: $dc_light;
            border-radius: 0;
            text-transform: uppercase;
            position: absolute;
            left: 0;
            top: -25px;
        }

        .more {
            font-size: 10px;

            .btn {
                width: 185px;
                padding: .75rem 0;
            }
        }
    }
}
</style>