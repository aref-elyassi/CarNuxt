<template>
     <div class="mysection">
        <div class="mycard">
             <img class="myimage" :src="require(`@/assets/images/${smallcard.image || 'car5.jpg'}`)" alt=""></img>
            <h4>{{smallcard.description}}</h4>
            <span>{{smallcard.time}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        props:['smallcard']
    }
</script>

<style scoped>

</style>