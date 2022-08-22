<template>
    <div class="container-fluid contain">  
        <div class="row">

            <nav class="navbar">
                <nuxt-link to="/">
                    
                    <img class="image" src="@/assets/images/logo.png" alt="logo-website">
                </nuxt-link>
            

                <div class="input">
                    <input type="text" placeholder="Search for cars and bikes">
                </div>
                   
                <div class="signin">
                    <nuxt-link to="/signin" class="router">
                        <img src="@/assets/icons/acc.png" alt="">
                            sing in
                    </nuxt-link>
                </div>
                
            </nav>
        
        </div>
        <div class="row contain-below">
            <nav class="second-navbar">
                <ul class="nav">
                    <li>
                        <nuxt-link class="router" to="/">Home</nuxt-link>

                    </li>
                    <li>
                        <nuxt-link class="router" to="/cars">Cars</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link class="router" to="/bikes">Bikes</nuxt-link>
                    </li>
                    <li>
                        <nuxt-link class="router" to="/signin">Sign in</nuxt-link>
                    </li>
                </ul>
            </nav>
        </div>   
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style  scoped>
li{
    list-style: none;
}
.second-navbar{
    width: 20%;
    display: flex;
    align-items: center;
    justify-content: center;
}
.contain-below{
    width: 100%;
      display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 10px ;
}
.nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
}
input{
    width: 25rem;
    height: 2.5rem;
    border-radius: 15px;
    border: 1px solid #707070;
    background: transparent;
}
input::placeholder{
    color: #707070;
    text-align: center;
    font-size:1.2em;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
.image{
    width: 10rem;
    object-fit: contain;
}
.contain{
    background: #26282b;
    width: 100%;
    margin: 0;
    display: flex;
    flex-direction: column;
 
}
.navbar{
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 5rem;
}
.router{
    color: #949393;
    text-decoration: none;
}
.router:hover{
    text-decoration: underline;
    color: rgb(255, 230, 4);
}


</style>