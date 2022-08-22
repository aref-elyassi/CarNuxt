<template>
    <div class="content">
        <img class="myimage" :src="require(`@/assets/images/${smallcard.image || 'car5.jpg'}`)" alt="">
        <h5>Name:{{smallcard.name}}</h5>
        <p>{{smallcard.description}}</p>
        <h3>Price:{{smallcard.price}}</h3>
    </div>
</template>

<script>
    export default {
        props:['smallcard']
    }
</script>

<style  scoped>
.content{
    display: flex;
    flex-direction: column;
    border: 1px solid #707070;
    border-radius: 10px;
    width: 20%;
    justify-content: space-between;
    background: rgba(49, 49, 49, 0.5);
    padding: 10px;
    color: gold;

}
.myimage{
    width: 15rem;
    height: 15rem;
    object-fit: contain;
}
</style>