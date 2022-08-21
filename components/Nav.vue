<template>
    <div class="contain">     
            <nav class="navbar">
                <div>
                    <img class="image" src="@/assets/images/logo.png" alt="logo-website">
                </div>

                <div class="input">
                    <input type="text">
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
    justify-content: space-between;
}
.router{
    color: #fff;
    text-decoration: none;
}

</style>