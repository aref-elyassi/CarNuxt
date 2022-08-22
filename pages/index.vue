<template>
  <div class="container-fluid contain">
    <div class="row">
      <nuxt-link to="/">
        <img class="image-main-section" src="@/assets/images/mainpic.png" alt="main picture">
      </nuxt-link>
    </div>
    <div class="row">
      <div class="after-nav">
        <div class="largecardsection">
         
          <nuxt-link class="router" to="/cars">View All Cars</nuxt-link>
          <LargeCard :largecard="largeCardinfo"/>
        </div>
        <div class="smallcardsection">
          <SmallCardDisplay  :smallcarddisplay="smallCardinfo"/>
        </div>
      </div>
    </div>
 <div class="row">
      <div class="after-nav2">
        <div class="smallcardsection">
          <SmallCardDisplayBike  :smallcarddisplaybike="smallCardinfoBike"/>
        </div>
        <div class="largecardsection2">
          <nuxt-link class="router" to="/bikes">View All Bikes</nuxt-link>
          <LargeCardBike :largecardbike="largeCardinfoBike"/>
        </div>
      </div>
    </div>

    
  </div>
</template>

<script>

import LargeCard from '../components/LargeCard.vue';
import {largeCardHome,largeCardHomeBike,smallCardHome,smallCardHomeBike} from '../assets/data.js'
import SmallCardDisplay from '../components/SmallCardDisplay.vue';
import LargeCardBike from '../components/LargeCardBike.vue';
import SmallCardDisplayBike from '../components/SmallCardDisplayBike.vue';

export default {
  name: 'IndexPage',
  components:{
    LargeCard,
    SmallCardDisplay,
    LargeCardBike,
    SmallCardDisplayBike
},
data(){
  return{
    largeCardinfo:largeCardHome,
    smallCardinfo:smallCardHome,
    largeCardinfoBike:largeCardHomeBike,
    smallCardinfoBike:smallCardHomeBike
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
.largecardsection{
  display: flex;
  justify-content: center;
  flex-direction: column-reverse;
  margin-left: 2rem;

}
.largecardsection2{
  display: flex;
  justify-content: center;
  flex-direction: column-reverse;
  margin-right: 2rem;

}
.smallcardsection{
  display: flex;
  align-items: center;
  justify-content: center;
}
.after-nav{
background: rgb(103,103,103);
background: linear-gradient(162deg, rgba(103,103,103,1) 0%, rgba(62,62,62,1) 44%, rgba(25,25,25,0.981127485173757) 100%);
display: flex;
align-items: center;
justify-content: space-between;
width: 100%;
}
.after-nav2{
background: rgb(103,103,103);
background: linear-gradient(300deg, rgba(103,103,103,1) 0%, rgba(62,62,62,1) 44%, rgba(25,25,25,0.981127485173757) 100%);
display: flex;
align-items: center;
justify-content: space-between;
width: 100%;
}
.router{
    color: #949393;
    text-decoration: none;
    width: 11rem;
    font-size: 1.5rem;
    margin-top: 3rem;
   
}
.router:hover{
    text-decoration: underline;
    color: rgb(255, 230, 4);
}

</style>
