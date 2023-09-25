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
        <div class="container">
            <a href="" class="btn btn-primary">current series</a>
        </div>
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

    .container {
        position: relative;

        a.btn {
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
            bottom: -20px;
        }
    }

}
</style>