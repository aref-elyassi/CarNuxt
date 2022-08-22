<template>
     <div class="mysection">
        <div class="mycard">
             <img class="myimage" :src="require(`@/assets/images/${smallcard.image || 'car5.jpg'}`)" alt="">
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
.myimage{
    object-fit: cover;
}
.mycard{
    display: flex;
    flex-direction: column;
    border: 1px solid #707070;
    border-radius: 10px;
    width: 20rem;
    color:#707070;
    padding: 10px;
    margin: 1rem;
}
</style>