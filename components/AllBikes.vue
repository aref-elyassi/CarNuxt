<template>
    <div class="allcars">
            <div class="content-all-cars">
            <img :src="require(`@/assets/images/${allbike.image}`)" alt="">
            <h3>{{allbike.name}}</h3>
            <p>{{allbike.description}}</p>
            <p>Price:{{allbike.price}}</p>
            <nuxt-link :to="`/bikes/${allbike.id}`" class="card-container btn btn-dark">Details</nuxt-link>      
            </div>

    </div>
</template>

<script>
    export default {
        props:['allbike']
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