<script>

export default {
    name: 'MenuItem',
    data() {
        return {}
    },
    props: {
        url: String,
        name: String,
        imgPath: String
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    },

}

</script>

<template>
    <li class="d-flex align-items-center p-3">
        <a :href="url" class="d-flex align-items-center">
            <div class="item_img">
                <img class="img-fluid" :src="getImageUrl(imgPath)" alt="">
            </div>
            <span>{{ name }}</span>
        </a>
    </li>
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

li>a {
    color: $dc_light;
    text-decoration: none;
    text-transform: uppercase;

    .item_img img {
        height: 60px;
        margin-right: 1rem;
    }
}
</style>