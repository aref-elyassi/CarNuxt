<template>
    <div class="container-fluid">
        <div class="row">
          <div class="form">
            <h1>Please Complete This Form</h1>
              <div class="mb-3">
                  <label for="exampleFormControlInput1" class="form-label">Name</label>
                    <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="john due">
                </div>
           
            <div class="mb-3">
                <label for="exampleFormControlInput1" class="form-label">Email address</label>
                <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
            </div>
            <div class="signin-out">
                <button class="btn btn-success">Log In</button>           
                <nuxt-link to="/signup" class="router">Don't Have acoount??  Please Create Account</nuxt-link>
            </div>
        
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style  scoped>
.container-fluid{
    background: #26282b;
}
.signin-out{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 60%;
}
input{
    background-color: #374245;
    border: 1px solid #707070;
}
input::placeholder{
    color:#cacaca ;
}
.form{
    border: 1px solid #cacaca;
    border-radius: 10px;
    padding: 20px;
    margin-top: 5rem;
    background: #374245;
    color:#e1dfdf
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