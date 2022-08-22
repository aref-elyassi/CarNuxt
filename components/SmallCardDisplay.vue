<template>
    <div>
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

<style lang="scss" scoped>

</style>