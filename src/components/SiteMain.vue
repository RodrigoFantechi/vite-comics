<script>
export default {
    name: 'SiteMain',
    data() {
        return {
            links: [
                {
                    image: '/assets/img/buy-comics-digital-comics.png',
                    link: 'DIGITAL COMICS'
                },
                {
                    image: '/assets/img/buy-comics-merchandise.png',
                    link: 'DC MERCHANDISE'
                },
                {
                    image: '/assets/img/buy-comics-shop-locator.png',
                    link: 'SUBSCRIPTION'
                },
                {
                    image: '/assets/img/buy-comics-subscriptions.png',
                    link: 'COMIC SHOP LOCATOR'
                },
                {
                    image: '/assets/img/buy-dc-power-visa.svg',
                    link: 'DC POWER VISA'
                },
            ],
            dcComics: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ],
            shop: [
                'shop DC',
                'Shop DC Collectibles',
            ],
            dc: [
                'Term Of Use',
                'Privacy policy (New)',
                'Ad Choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Woekshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us',
            ],
            sites: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa',
            ],


        }
    }
}
</script>

<template>
    <section class="black_banner">
        <div class="container p-4 ">
            <p> --> Content goes Here &lt;-- </p>
        </div>
    </section>
    <section class="linked">
        <div class="container">
            <div class="row row-cols-5">
                <div class="col d-flex align-items-center p-5" v-for="item in links">
                    <img :src="'/src' + item.image" alt="">
                    <p class="mb-0 ms-3">{{ item.link }}</p>
                </div>
            </div>
        </div>
    </section>
    <section class="list">
        <div class="container d-flex justify-content-between">
            <div class="col-5">
                <div class="container py-5">
                    <div class="row row-cols-3">
                        <div class="col">
                            <ul>
                                <li><a href="#">
                                        <h5 class="mb-3 text-light">DC COMICS</h5>
                                    </a></li>
                                <li v-for="items in dcComics" class="font"><a href="#">{{ items }}</a></li>
                                <li><a href="#">
                                        <h5 class="my-3 text-light">SHOP</h5>
                                    </a></li>
                                <li v-for="items in shop" class="font"><a href="#">{{ items }}</a></li>
                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li><a href="#">
                                        <h5 class="mb-3 text-light">DC</h5>
                                    </a></li>
                                <li v-for="items in dc" class="font"><a href="#">{{ items }}</a></li>
                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li><a href="#">
                                        <h5 class="mb-3 text-light">SITES</h5>
                                    </a></li>
                                <li v-for="items in sites" class="font"><a href="#">{{ items }}</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class=" col-7 logoImage"></div>
        </div>
    </section>

</template>

<style lang="scss" scoped>

</style>