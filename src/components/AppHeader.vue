<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            activeLink: 1,
            linkList: [
                {
                    url: '#',
                    name: 'Characters'
                },
                {
                    url: '#',
                    name: 'Comics'
                },
                {
                    url: '#',
                    name: 'Movies'
                },
                {
                    url: '#',
                    name: 'TV'
                },
                {
                    url: '#',
                    name: 'Games'
                },
                {
                    url: '#',
                    name: 'Collectibles'
                },
                {
                    url: '#',
                    name: 'Videos'
                },
                {
                    url: '#',
                    name: 'Fans'
                },
                {
                    url: '#',
                    name: 'News'
                },
                {
                    url: '#',
                    name: 'Shop'
                },
            ]
        }
    }
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
                    <a v-for="(item, i) in linkList" :class="activeLink === i ? 'active' : ''" class="nav-item nav-link"
                        :href="item.url">{{ item.name }}</a>
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