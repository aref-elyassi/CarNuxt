<template>
    <div>
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

<style lang="scss" scoped>

</style>