<template>
    <div class="allcars2">
        <AllBikes 
            v-for="bikes in product" :key="bikes.id"
        :allbike="bikes"/>
</div>
</template>

<script>
import { mapGetters } from 'vuex';
import AllBikes from '../../components/AllBikes.vue';
    export default {
    computed: {
        product() {
            return this.$store.getters.allBikes;
        }
    },
    components: { AllBikes }
}
</script>

<style  scoped>
.allcars2{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-evenly;
 background: #26282b;
}
</style>