<script>

export default {
    name: 'FooterLinks',
    data() {
        return {
            comicsMenu: {
                name: 'Dc Comics',
                linkList: [
                    {
                        name: 'Characters',
                        url: '#'
                    },
                    {
                        name: 'Comics',
                        url: '#'
                    },
                    {
                        name: 'Movies',
                        url: '#'
                    },
                    {
                        name: 'TV',
                        url: '#'
                    },
                    {
                        name: 'Games',
                        url: '#'
                    },
                    {
                        name: 'Videos',
                        url: '#'
                    },
                    {
                        name: 'News',
                        url: '#'
                    },
                ]
            },
            shopMenu: {
                name: 'Shop',
                linkList: [
                    {
                        name: 'Shop DC',
                        url: '#'
                    },
                    {
                        name: 'Shop DC Collectibles',
                        url: '#'
                    }
                ]
            },
            dcMenu: {
                name: 'DC',
                linkList: [
                    {
                        name: 'Terms Of Use',
                        url: '#'
                    },
                    {
                        name: 'Privacy Policy (New)',
                        url: '#'
                    },
                    {
                        name: 'Ad Choices',
                        url: '#'
                    },
                    {
                        name: 'Advertising',
                        url: '#'
                    },
                    {
                        name: 'Job',
                        url: '#'
                    },
                    {
                        name: 'Subscriptions',
                        url: '#'
                    },
                    {
                        name: 'Talent Workshops',
                        url: '#'
                    },
                    {
                        name: 'CPSC Certificates',
                        url: '#'
                    },
                    {
                        name: 'Ratings',
                        url: '#'
                    },
                    {
                        name: 'Shop Help',
                        url: '#'
                    },
                    {
                        name: 'Contact Us',
                        url: '#'
                    }
                ]
            },
            sitesMenu: {
                name: 'Sites',
                linkList: [
                    {
                        name: 'DC',
                        url: '#'
                    },
                    {
                        name: 'MAD Megazine',
                        url: '#'
                    },
                    {
                        name: 'DC Kids',
                        url: '#'
                    },
                    {
                        name: 'DC Universe',
                        url: '#'
                    },
                    {
                        name: 'DC Power Visa',
                        url: '#'
                    }
                ]
            }
        }
    }
}

</script>

<template>
    <div id="useful_links" class="row text-light">

        <div class="row">
            <div class=" col-4">
                <ul class="list-unstyled">
                    <h5 class="text-uppercase">{{ comicsMenu.name }}</h5>
                    <li v-for="item in comicsMenu.linkList">
                        <a :href="item.url" class="text-decoration-none text-light">{{ item.name }}</a>
                    </li>
                </ul>

                <ul class="list-unstyled mt-5">
                    <h5 class="text-uppercase">{{ shopMenu.name }}</h5>
                    <li v-for="item in shopMenu.linkList">
                        <a :href="item.url" class="text-decoration-none text-light">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <!-- /.col-4 -->
            <div class="col-4">
                <ul class="list-unstyled">
                    <h5 class="text-uppercase">{{ dcMenu.name }}</h5>
                    <li v-for="item in dcMenu.linkList">
                        <a :href="item.url" class="text-decoration-none text-light">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <!-- /.col-4 -->
            <div class="col-4">
                <ul class="list-unstyled">
                    <h5 class="text-uppercase">{{ sitesMenu.name }}</h5>
                    <li v-for="item in sitesMenu.linkList">
                        <a :href="item.url" class="text-decoration-none text-light">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <!-- /.col-4 -->
        </div>




    </div>
</template>

<style lang="scss" scoped>
#useful_links {
    .col-4 {
        ul.list-unstyled {
            h5 {
                font-size: 15px;
            }

            li a {
                font-size: 10px;
            }
        }
    }
}
</style>