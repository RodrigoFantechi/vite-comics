<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            menuNav: [
                {
                    text: 'CHARACTERS',
                    href: '#'
                },
                {
                    text: 'COMICS',
                    href: '#'
                },
                {
                    text: 'MOVIES',
                    href: '#'
                },
                {
                    text: 'TV',
                    href: '#'
                },
                {
                    text: 'GAMES',
                    href: '#'
                },
                {
                    text: 'COLLECTIBLES',
                    href: '#'
                },
                {
                    text: 'VIDEOS',
                    href: '#'
                },
                {
                    text: 'FANS',
                    href: '#'
                },
                {
                    text: 'NEWS',
                    href: '#'
                },
                {
                    text: 'SHOP',
                    href: '#'
                },
            ]
        }
    }
}
</script>

<template>
    <nav class="navbar navbar-expand-lg p-3">
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                    <li class="nav-item my-1" v-for="item in menuNav">
                        <div class="links ms-auto ">
                            <a class="mx-3" :href="item.href">
                                {{ item.text }}
                            </a>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </nav>




</template>

<style lang="scss" scoped>

</style>