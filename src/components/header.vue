<template>
    <div class="header">
        <b-navbar toggleable="md" type="light" fixed="top">
            <div class="container pt-n1">
                <b-navbar-brand>
                    <router-link class="navbar-brand font-weight-bold txt-size-n1" to="#" exact>
                        <img src="../assets/logo1.png" class="d-inline-block" alt="logo">
                        tinyone
                    </router-link>
                </b-navbar-brand>

                <b-navbar-toggle target="nav-collapse" class="font-weight-bold"></b-navbar-toggle>

                <b-collapse id="nav-collapse" is-nav>
                    <b-navbar-nav class="ml-auto">
                        <b-nav-item>
                            <router-link class="nav-link text-dark font-weight-bold" to="#" exact>Features</router-link>
                        </b-nav-item>
                        <b-nav-item>
                            <router-link class="nav-link text-dark font-weight-bold" to="#" exact>Support</router-link>
                            </b-nav-item>
                        <b-nav-item>
                            <router-link class="nav-link text-dark font-weight-bold" to="#" exact>Blog</router-link>
                        </b-nav-item>
                    </b-navbar-nav>
                </b-collapse>
            </div>
        </b-navbar>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                
            }
        }
    } 
</script>

<style scoped>

b-navbar{
    background-color: #fcdb00;
}
.navbar-light .navbar-toggler{
    border:none;
    color: #000;
}
button:focus{
    outline: none;
}
.navbar-toggler:after{
    content:"  Menu";
    font-size: 1.5rem;
}
.pt-n1{
    padding-top: 1.5rem;
}
.navbar-expand-md{
    padding: 0 1rem;
}
.txt-size-n1{
    font-size: 2rem;
}
.nav-link{
    font-size: 1.375rem;
}
.txt-color-black{
    color:black;
}
.header{
    background-color: #fcdb00;
}
.container{
    max-width: 50%;   
}
.nav-link:hover{
    color: #fff !important;
}
.d-inline-block{
    width: 40px;
    height: 40px;
}
.fixed-top{
    position: relative;
}

/*MEDIA*/
@media only screen and (max-width: 1680px)  {
    .container{
        max-width: 60%;   
    }
}
@media only screen and (max-width: 1440px)  {
    .container{
        max-width: 70%;   
    }
}
@media only screen and (max-width: 1024px)  {
    .container{
        max-width: 80% ; 
    }
    .pt-n1{
        padding-top: 0.5rem !important;
    }
    .txt-size-n1{
        font-size: 1.75rem;
    }
    .nav-link{
        font-size: 1.25rem;
    }
}
@media only screen and (max-width: 768px)  {
    .container{
        max-width: 90% ;   
    }
    .pt-n1{
        padding-top: 0.5rem !important;
    }
    .nav-item{
        text-align: center;
    }
    .nav-item:hover{
        background:rgba(255, 234, 0, 0.5);
        margin: 0 -10%;
    }
    .navbar-toggler:after{
        content:"  Menu";
        font-size: 1.25rem;
    } 
    .txt-size-n1{
        font-size: 1.5rem;
    }
    .fixed-top{
        position: fixed;
        background: rgb(252, 219, 0, 0.9);    
    }  
}
@media only screen and (max-width: 703px)  {
    .container{
        max-width: 95%;   
    }
    .pt-n1{
        padding-top: 0 !important;
    }
}
@media only screen and (max-width: 414px)  {
    .container{
        max-width: 100%;   
    }
    .pt-n1{
        padding-top: 0 !important;
    }   
}
</style>