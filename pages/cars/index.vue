<template>
    <div class="allcars2">
        <AllCars 
            v-for="cars in product" :key="cars.id"
        :allcar="cars"/>
</div>
</template>

<script>
import { mapGetters } from 'vuex';
import AllCars from '../../components/AllCars.vue';
    export default {
    computed: {
        product() {
            return this.$store.getters.allCars;
        }
    },
    components: { AllCars }
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