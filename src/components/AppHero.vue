<script>

export default {
    name: 'AppHero',
    props: {
        imgPath: String
    },
    components: {
    }
}
</script>

<template>
    <section id="app_hero">
        <img :src="imgPath">
    </section>
    <!-- /#app_hero -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#app_hero {

    img {
        width: 100%;
        height: 400px;
        object-fit: cover;
        object-position: top;
    }

}
</style>