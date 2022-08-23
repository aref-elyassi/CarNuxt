<template>
    <div class="footer">
        <div>
            <ul>
                        <li>Car&Bike</li>
                        <li>
                            <nuxt-link class="router" to="/">About Us</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link class="router" to="/">New Cars</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Used Cars</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">New Bikes</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Used Bikes</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Sell Your Cars</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Privacy Policy</nuxt-link>
                        </li>
                    </ul>
                </div>
                 <div>
                     <ul>
                        <li>Popular Car Brands</li>
                        <li>
                            <nuxt-link class="router" to="/">Maruti Suzuki</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link class="router" to="/">Hyundai</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Tata</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Volkswagen</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Honda</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Mahindra</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Kia</nuxt-link>
                        </li>
                    </ul>
                </div>
                        
                    <div>
                        <ul>
                        <li>Popular Car Models</li>
                        <li>
                            <nuxt-link class="router" to="/">Mahindra XUV 700</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link class="router" to="/">Kia Seltos</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Mahindra Thar</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Tata Nexon</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Kia Sonet</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Tata Punch</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">MG Hector</nuxt-link>
                        </li>
                    </ul>
                </div>
                 <div>
                     <ul>
                        <li>Popular Bike Brands</li>
                        <li>
                            <nuxt-link class="router" to="/">Royal Enfield</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link class="router" to="/">Honda</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">KTM</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Bajaj</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Yamaha</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">TVS</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Hero</nuxt-link>
                        </li>
                    </ul>
                </div>
                   <div>
                       <ul>
                        <li>Popular Bike Models</li>
                        <li>
                            <nuxt-link class="router" to="/">Royal Enfield Classic 350</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link class="router" to="/">Yamaha MT-15</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Bajaj Pulsar 220</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">KTM RC 200</nuxt-link>
                        </li>
                         <li>
                            <nuxt-link class="router" to="/">Hero Splendor Plus</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Bajaj Pulsar 150</nuxt-link>
                        </li>
                          <li>
                            <nuxt-link class="router" to="/">Honda CB Shine</nuxt-link>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>

                    </ul>
                </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style  scoped>
.router{
    color: #949393;
    text-decoration: none;
   
  
   
}
.router:hover{
    text-decoration: underline;
    color: rgb(255, 230, 4);
}
.footer{
    display: flex;
    justify-content: space-evenly;
    background: #26282b;
    border-top: 1px solid #707070;
    padding-top: 20px;
}

.footer>div{
    display: flex;
    flex-direction: column;
    align-items: center;
}
.footer>div>ul{
    display: flex;
    flex-direction: column;
}
li{
    list-style: none;
    color: gold;
    
}
ul>li:first-child{
    border-bottom: 1px solid gold;
}
</style>