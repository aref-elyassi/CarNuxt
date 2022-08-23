<template>
    <div class="allcars">
            <div class="content-all-cars">
            <img :src="require(`@/assets/images/${allcar.image}`)" alt="">
            <h3>{{allcar.name}}</h3>
            <p>{{allcar.description}}</p>
            <p>Price:{{allcar.price}}</p>
            <nuxt-link :to="`/cars/${allcar.id}`" class="card-container btn btn-dark">Details</nuxt-link>      
            </div>
    </div>
</template>

<script>
    export default {
        props:['allcar']
    }
</script>

<style  scoped>
.allcars{
    display: flex;
}
.content-all-cars{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    border: 1px solid #707070;
    border-radius: 10px;
    width: 20rem;
    color: #707070;
    margin-top: 2rem;
    margin-bottom: 1rem;
    padding-bottom: 10px;
}
.content-all-cars>img{
    width: 19rem;
    height: 20rem;
    border-radius: 10px;
}
</style>