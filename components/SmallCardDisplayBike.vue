<template>
    <div class="cs">
        <SmallCardBike v-for="smallcardbike in smallcarddisplaybike" :key="smallcardbike.id"
        :smallcardbike="smallcardbike"
        />
    </div>
</template>

<script>
import SmallCardBike from './SmallCardBike.vue';
    export default {
    components: { SmallCardBike },
    props:['smallcarddisplaybike']

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