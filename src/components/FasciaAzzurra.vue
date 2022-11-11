<script>
export default {
    name: 'FasciaAzzurra',
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
            
        }
    }
}
</script>

<template>
    
        <section class="linked">
            <div class="container">
                <div class="row row-cols-5">
                    <div class="col d-flex align-items-center py-5" v-for="item in links">
                        <img :src="'/src' + item.image" alt="">
                        <p class="mb-0 ms-3"><a href="#">{{ item.link }}</a></p>
                    </div>
                </div>
            </div>
        </section>
 
</template>

<style lang="scss" scoped>

</style>