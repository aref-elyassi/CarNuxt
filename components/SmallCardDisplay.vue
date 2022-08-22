<template>
    <div class="cs">
        <SmallCard 
        v-for="smallcard in smallcarddisplay" :key="smallcard.id"
        :smallcard="smallcard"/>
    </div>
</template>

<script>
import SmallCard from './SmallCard.vue';
    export default {
    props: ["smallcarddisplay"],
    components: { SmallCard }
}
</script>

<style  scoped>
.cs{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}
</style>