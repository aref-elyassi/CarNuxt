<template>
  <div class="container-fluid contain">
    <div class="row">
      <nuxt-link to="/">
        <img class="image-main-section" src="@/assets/images/mainpic.png" alt="main picture">
      </nuxt-link>
    </div>
    <div class="row">
      <div class="after-nav">
        <LargeCard :largecard="largeCardinfo"/>
      </div>
    </div>
  </div>
</template>

<script>

import LargeCard from '../components/LargeCard.vue';
import largeCardHome from '../assets/data.js'
export default {
  name: 'IndexPage',
  components:{
    LargeCard,
},
data(){
  return{
    largeCardinfo:largeCardHome
  }
}
  
}
</script>
<style scoped>
*{
  margin: 0;
  padding: 0;
}

.image-main-section{
  width:100%;
  filter:brightness(80%)
}

.after-nav{
background: #26282b;

}
</style>
