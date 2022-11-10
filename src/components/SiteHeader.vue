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
    <div class="container">
        <nav class="d-flex justify-content-between align-items-center p-2">
            <img src="../assets/img/dc-logo.png" alt="">
            <div class="links">
                <a  v-for="item in menuNav" :href="item.href" :class="item.text === 'COMICS' ? 'active' : ''">
                    {{ item.text }}
                </a>
            </div>
        </nav>
    </div>


</template>

<style lang="scss" scoped>

</style>