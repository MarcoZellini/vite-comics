<script>
import MainMenu from './MainMenu.vue'

export default {
    name: 'AppMain',
    components: {
        MainMenu
    }
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