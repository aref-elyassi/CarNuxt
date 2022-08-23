<template>
<div class="content">
    <div class="details">
        <div class="text-details">            
            <h1>Name:{{product.name}}</h1>
            <p>{{product.description}}</p>
            <p>{{product.description2}}</p>
            <h1>Price:{{product.price}}</h1>
         </div>
            <img :src="require(`@/assets/images/${product.image}`)" alt="">
    </div>
</div>
</template>

<script>
import { mapGetters } from 'vuex';
    export default {
         computed: {
            product() {
                return this.$store.getters.getBikeById(this.$route.params.id);
            }
    }
    }
</script>

<style  scoped>
.content{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
 background: #26282b;
}
.details{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 80%;
    height: 80vh;
    border: 1px solid #707070;
    padding: 20px;
    border-radius: 10px;
    color: #707070;
}
img{
    width: 40rem;
    height: 30rem;
}
</style>