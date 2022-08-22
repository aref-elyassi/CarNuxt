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
        <SmallCardDisplay :smallcarddisplay="smallCardinfo"/>
      </div>
    </div>
  </div>
</template>

<script>

import LargeCard from '../components/LargeCard.vue';
import {largeCardHome,smallCardHome} from '../assets/data.js'
import SmallCardDisplay from '../components/SmallCardDisplay.vue';
export default {
  name: 'IndexPage',
  components:{
    LargeCard,
    SmallCardDisplay
},
data(){
  return{
    largeCardinfo:largeCardHome,
    smallCardinfo:smallCardHome
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
height: 60vh;
display: flex;
align-items: center;

}
</style>
