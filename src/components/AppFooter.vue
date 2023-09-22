<script>
import FooterTop from './FooterTop.vue'
import FooterBottom from './FooterBottom.vue'

export default {
    name: 'AppFooter',

    components: {
        FooterTop,
        FooterBottom
    }
}
</script>

<template>
    <footer id="app_footer">

        <FooterTop />

        <FooterBottom />

    </footer>
    <!-- /#app_footer -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#app_footer {}
</style>