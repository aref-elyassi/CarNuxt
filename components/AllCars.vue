<template>
    <div class="allcars">
            <div class="content-all-cars">
            <img :src="require(`@/assets/images/${allcar.image}`)" alt="">
            <h3>{{allcar.name}}</h3>
            </div>

    </div>
</template>

<script>
    export default {
        props:['allcar']
    }
</script>

<style lang="scss" scoped>

</style>