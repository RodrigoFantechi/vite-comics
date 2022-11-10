<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMain from './components/SiteMain.vue';
import Sitefooter from './components/SiteFooter.vue';

export default {
  components: {
    SiteHeader,
    SiteMain,
    Sitefooter
  }
}
</script>

<template>
  <SiteHeader />
  <SiteMain />
  <Sitefooter />
</template>

<style lang="scss" scoped>

</style>
