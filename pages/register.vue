<template>
    <div class="container col-md-6 mt-5">
        <div class="card">
            <div class="card-header">
                Register
            </div>
            <div class="card-body">
                <form>
                <div class="form-group">
                    <label>Email address</label>
                    <input type="email" class="form-control" placeholder="Enter Your Email Address" autofocus>
                    <small class="form-text text-danger">Error message here.</small>
                </div>
                <div class="form-group">
                    <label>Password</label>
                    <input type="password" class="form-control" placeholder="Password">
                    <small class="form-text text-danger">Error message here.</small>
                </div>
           
                <button type="submit" class="btn btn-primary">Register</button>
                </form>
                <br/>
                <p>Already have an account? <nuxt-link to="/login">Login</nuxt-link></p>
            </div>
        </div>
        
    </div>
</template>