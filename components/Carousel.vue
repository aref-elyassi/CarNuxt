<template>
    <div class="mycarousel">
        <SmallCardCarousel
        v-for="sm in smallCardinfo" :key="sm.id"
         :smallcard="sm"/>
    </div>
</template>

<script>
import {smallCardHome} from '../assets/data.js'
import SmallCardCarousel from './SmallCardCarousel.vue';
    export default {
    data() {
        return {
            smallCardinfo: smallCardHome,
        };
    },
    components: { SmallCardCarousel }
}
</script>

<style  scoped>
.mycarousel{
    display: flex; 
    justify-content: space-evenly;
    align-items: center;

}
</style>