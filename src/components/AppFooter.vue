<script>
import FooterTop from './FooterTop.vue'

export default {
    name: 'AppFooter',

    components: {
        FooterTop
    }
}
</script>

<template>
    <footer id="app_footer">

        <FooterTop />
        <section id="others">
            <!-- Bottone signup -->

            <!-- Lista di social -->
        </section>
    </footer>
    <!-- /#app_footer -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#app_footer {}
</style>