<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
    <header id="app_header">
        <div class="container">
            <nav class="navbar navbar-expand justify-content-between p-0">
                <a class="navbar-brand" href="#">
                    <img class="img-fluid" src="../assets/img/dc-logo.png" alt="DC_logo">
                </a>

                <div class="nav navbar-nav gx-3">
                    <a class="nav-item nav-link" href="#">Characters</a>
                    <a class="nav-item nav-link active" href="#">Comics</a>
                    <a class="nav-item nav-link" href="#">Movies</a>
                    <a class="nav-item nav-link" href="#">Tv</a>
                    <a class="nav-item nav-link" href="#">Games</a>
                    <a class="nav-item nav-link" href="#">Collectibles</a>
                    <a class="nav-item nav-link" href="#">Videos</a>
                    <a class="nav-item nav-link" href="#">Fans</a>
                    <a class="nav-item nav-link" href="#">News</a>
                    <a class="nav-item nav-link" href="#">Shop</a>
                </div>
            </nav>
        </div>
    </header>
    <!-- /#app_header -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/partials/variables' as *;

#app_header {
    background-color: $dc_light;

    .navbar-brand {

        img {
            width: 80%;
        }
    }

    a.nav-item {
        text-transform: uppercase;
        font-family: 'Encode Sans', sans-serif;
        font-size: 800;
        padding: 3rem .5rem;
        font-size: .8rem;
        color: $dc_dark_soft;

        &.active {
            color: $dc_primary;
            border-bottom: 5px solid $dc_primary;
        }

    }
}
</style>