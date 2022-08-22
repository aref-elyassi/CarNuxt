<template>
    <div class="mysection">
        <div class="mycard">
             <img class="myimage" :src="require(`@/assets/images/${largecardbike.image || 'car5.jpg'}`)" alt="">
            <h4>{{largecardbike.description}}</h4>
            <span>{{largecardbike.time}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        props:['largecardbike']
    }
</script>


<style  scoped>
.myimage{
   object-fit: cover;
}
.mycard{
    display: flex;
    flex-direction: column;
    align-items: center;
border: 1px solid #707070;
border-radius: 10px;
color: #707070;

}


</style>