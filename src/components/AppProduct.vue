<script>

export default {
    name: 'AppProduct',

    props: {
        href: String,
        title: String
    }
}

</script>

<template>
    <div id="product">
        <img class="img-fluid" :src="href" alt="">
        <h6>{{ title }}</h6>
    </div>
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;


#product {
    color: $dc_light;
    text-transform: uppercase;

    img {
        aspect-ratio: 1/1;
        object-fit: cover;
        object-position: top;
        margin-bottom: 1.5rem;
    }

}
</style>