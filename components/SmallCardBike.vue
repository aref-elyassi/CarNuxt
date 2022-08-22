<template>
      <div class="mysection">
        <div class="mycard">
             <img class="myimage" :src="require(`@/assets/images/${smallcardbike.image || 'bike5.jpg'}`)" alt="">
            <h4>{{smallcardbike.description}}</h4>
            <span>{{smallcardbike.time}}</span>
           
        </div>
    </div>
</template>

<script>
    export default {
        props:['smallcardbike']
    }
</script>

<style scoped>
.myimage{
    object-fit: cover;
    border-radius: 10px;
}
.mycard{
    display: flex;
    flex-direction: column;
    border: 1px solid #707070;
    border-radius: 10px;
    width: 20rem;
    color:#707070;
    padding: 10px;
    margin: 5px;
}
</style>