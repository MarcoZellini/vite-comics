<script>
export default {
    name: 'AppButton'
}
</script>

<template>
    <a class="btn text-uppercase d-flex align-items-center py-2">sign-up now!</a>
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

a {
    border: 2px solid $dc_primary;
    border-radius: 0;
    color: $dc_light;
}
</style>