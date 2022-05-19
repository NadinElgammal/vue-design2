<template>
    <section>
        <div class="container">
            <div class="lhs">
                <a href="#"><span class="text">Infeluncers</span></a>
                <a href="#"><span class="text">Details</span></a>
                <a href="#"><span class="text">Services</span></a>
                <a href="#"><span class="text">Statistics</span></a>
                <a href="#"><span class="text">Payemnts</span></a>
            </div>
            <div class="rhs">
                <button class="btn btn-1">Settings</button>
                <button class="btn btn-2">Export</button>
            </div>
        </div>
        <br>
        <div class="social-media">
                <button class="bttn insta"><i class="fa-brands fa-instagram"></i></button>
                <button class="bttn facebook"><i class="fa-brands fa-facebook-f"></i></button>
                <button class="bttn youtube"><i class="fa-brands fa-youtube"></i></button>
                <button class="bttn twitter"><i class="fa-brands fa-twitter"></i></button>
        </div>
    </section>
</template>

<script>
export default {
    name:"Tabs",
}
</script>

<style scoped>
    .container{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items:start;
    }
    .lhs{
        display: flex;
        gap: 60px;
        align-items: center;
    }
    .text{
        color:#b4b4b4;
    }
    a:link{
        text-decoration: none;
    }
    a:before{
        content: "";
        position: absolute;
        background-color: #0164fb;
        height: 3px;
        width: 0;
        /* left: 115px; */
        bottom: 810px;
        transition: 0.3s;
        
    }
    a:hover:before{
        width: 70px;
        font-weight: bold;
    }
    .rhs{
        display: flex;
        gap: 20px;
    }
    .btn-1{
        background-color: #F2F7FF;
        color:#0164fb;
        font-weight: bold;
    }
    .btn-2{
        background-color: #0164fb;
        color: white;
        font-weight: bold;
    }
    .btn{
        width: 200px;
        height: 50px;
        border-radius: 10px;
    }
    .social-media{
        box-shadow: 20px;
        margin-left: 30px;
    }
    .facebook ,.insta ,.youtube ,.twitter{
        font-size: 20px;
        padding: 15px;
    }
    .bttn{
        width: 200x;
        height: 60px;
        box-shadow: 20px;
    }
</style>