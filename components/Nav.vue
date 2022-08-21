<template>
    <div class="container-fluid contain">     
            <nav class="navbar">
                <div>
                    <img class="image" src="@/assets/images/logo.png" alt="logo-website">
                </div>

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
</template>

<script>
    export default {
        
    }
</script>

<style  scoped>
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
 
}
.navbar{
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 5rem;
}
.router{
    color: #707070;
    text-decoration: none;
}

</style>