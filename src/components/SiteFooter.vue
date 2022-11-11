<script>
export default {
    name: 'Sitefooter',
    data() {
        return {
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
    },
}
</script>

<template>
    <footer id="site-footer">
        <section class="list">
            <div class="container d-flex justify-content-between">
                <div class="col-5">
                    <div class="container py-5">
                        <div class="row row-cols-3">
                            <div class="col">
                                <ul>
                                    <li><a href="#">
                                            <h4 class="mb-3 text-light">DC COMICS</h4>
                                        </a></li>
                                    <li v-for="items in dcComics" class="font"><a href="#">{{ items }}</a></li>
                                    <li><a href="#">
                                            <h4 class="my-3 text-light">SHOP</h4>
                                        </a></li>
                                    <li v-for="items in shop" class="font"><a href="#">{{ items }}</a></li>
                                </ul>
                            </div>
                            <div class="col">
                                <ul>
                                    <li><a href="#">
                                            <h4 class="mb-3 text-light">DC</h4>
                                        </a></li>
                                    <li v-for="items in dc" class="font"><a href="#">{{ items }}</a></li>
                                </ul>
                            </div>
                            <div class="col">
                                <ul>
                                    <li><a href="#">
                                            <h4 class="mb-3 text-light">SITES</h4>
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
        <section class="allSocials">
            <div class="container d-flex justify-content-between">
                <div class="my_btn">SIGN-UP NOW!</div>
                <div class="social d-flex align-items-center">
                    <h6 class="blue me-3">FOLLOW US</h6>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </div>
            </div>
        </section>
    </footer>
    <!-- /#site-footer -->
</template>

<style lang="scss" scoped>

</style>
