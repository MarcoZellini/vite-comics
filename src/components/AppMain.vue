<script>
import AppHero from './AppHero.vue'
import MainMenu from './MainMenu.vue'

export default {
    name: 'AppMain',
    components: {
        MainMenu,
        AppHero
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

        <MainMenu />

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
}
</style>