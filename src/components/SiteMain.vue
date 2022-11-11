<script>
import FasciaAzzurra from './FasciaAzzurra.vue';
import Tumbler from './Tumbler.vue';
import tumblers from '../data/tumblers.js';
export default {
    name: 'SiteMain',
    components: {
        Tumbler,
    FasciaAzzurra,
  },
  data(){
        return{
            tumblers: tumblers,
        }
    }
}


</script>

<template>
    <main id="site-main">
        <section class="jumbotron"></section>
        <section class="my_grid">
            <div class="container position-relative">
                <div class="my_btn">CURRENT SERIES</div>
                <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-xxl-6 g-3 py-4">

                    <Tumbler v-for="item in tumblers" 
                    :img="item.thumb"
                    :title="item.series"
                    />
                </div>

            </div>


        </section>
        <FasciaAzzurra />
    </main>
    <!-- /#site-main -->
</template>

<style lang="scss" scoped>

</style>