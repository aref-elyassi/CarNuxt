<template>
    <div class="mysection">
        <div class="mycard">
             <img class="myimage" :src="require(`@/assets/images/${largecard.image || 'car5.jpg'}`)" alt="">
            <h4>{{largecard.description}}</h4>
            <span>{{largecard.time}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        name:'LargeCard',
        props:['largecard']
        
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
background: #343434;
color: #707070;

}


</style>