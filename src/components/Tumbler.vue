
<script>
export default {
    props:{
        img: String,
        title: String,
    }
}
</script>




<template>
    <div class="col">
        <div class="my_card text-center">
            <div class="image_card text-center">
                <img :src="img" :alt="title">
            </div>
            <h6 class="mt-3">{{title}}</h6>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    
</style>