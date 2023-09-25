<script>
import menuItems from '../menu_items.js'
import MenuItem from './MenuItem.vue'

export default {

    name: 'MainMenu',
    data() {
        return {
            menuItems
        }
    },

    components: {
        MenuItem
    }
}

</script>

<template>
    <section id="main_menu">
        <div class="container">
            <ul class="list-unstyled d-flex justify-content-around align-items-center py-5 m-0">


                <MenuItem v-for="item in menuItems" :imgPath="item.imgPath" :name="item.name" :url="item.url" />


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
}
</style>