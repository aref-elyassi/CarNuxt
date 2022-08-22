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
<div class="row">
  <div class="content_after_cards">
    <section class="section1">
        <div class="question">
          <h3>Question of Day</h3>
          <hr>
          <h4>What is your take on making 6 Airbags standard for all cars?</h4>
          <div class="myBtn">
            <button>Yes,Safety first</button>
            <button>No,Not Required</button>
          </div>
        </div>
    </section>
   
   <section class="section2">
        <div class="question">
          <h3>Cars And Bike</h3>
          <hr>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia quisquam omnis neque libero delectus odio ducimus facilis commodi illum. Esse veniam minus ipsa quas adipisci unde id iusto enim sit blanditiis voluptate iste dolor harum velit eaque perferendis architecto in, corporis excepturi accusamus nemo et illo. Non corporis dolor assumenda.</p>
         
        </div>
    </section>
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
.question{
  display: flex;
  flex-direction: column;
  width: 50%;
  border:1px solid #3a3a3a;
  border-radius: 15px;
  padding: 15px;
  box-shadow: 1px 1px 1px 1px;
  margin: 2rem;
}
.myBtn{
  display: flex;
  justify-content: space-evenly;
  margin-top: 10px;
}
.myBtn>button{
  background: transparent;
  border: 1px solid gold;
  border-radius: 10px;
  transition: .5s ease-in-out all;
  padding: 5px;
  color: gold;
}
.myBtn>button:hover{
  border: 1px solid #707070;
}
.section1{
  width: 50%;
}
.section1 .question{
  color: gold;
}
.section2{
  width: 50%;
  display: flex;
  justify-content: right;
}
.section2 .question{
  color: gold;
}
.section2 .question>p{
text-align: justify;
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
.content_after_cards{
  width: 100%;
  background-image:url('../assets/images/car13.png'),linear-gradient(162deg, rgba(148,147,147,1) 0%, rgba(68,67,67,1) 51%, rgba(37,37,37,1) 100%); ;
  background-repeat: no-repeat;
  height: 80vh;
  background-position: center;
  display: flex;
  align-items: center;
}

</style>
