<template>
    <div>
            <h1>{{product.name}}</h1>
    </div>
</template>

<script>
import { mapGetters } from 'vuex';
    export default {
         computed: {
            product() {
                return this.$store.getters.getCarById(this.$route.params.id);
            }
    }
    }
</script>

<style lang="scss" scoped>

</style>