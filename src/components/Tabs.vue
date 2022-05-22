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
                <button class="btnn btn-1">Settings</button>
                <button class="btnn btn-2">Export</button>
            </div>
        </div>
        <br>
        <div class="cont">
            <div class="container2">
                <div class="social-media shadow-3">
                    <div class="bttn insta shadow-inner" style="background:linear-gradient(100deg,#E4914C,#C74D7B) ; color:#FFFFFF"><i class="fa-brands fa-instagram" ></i></div>
                    <div class="bttn facebook"><i class="fa-brands fa-facebook-f" style="color:#395798"></i></div>
                    <div class="bttn youtube"><i class="fa-brands fa-youtube" style="color:#FF0000"></i></div>
                    <div class="bttn twitter"><i class="fa-brands fa-twitter" style="color:#149EF2"></i></div>
                </div>
                <div class="option shadow-3">
                    <div class="post shadow-3">
                        <div>
                            <i class="fa-regular fa-image"></i>
                        </div>
                        <div>
                            <span>Post</span>
                        </div>
                    </div>
                    <div class="story">
                        <div>
                            <i class="fa-solid fa-image-portrait"></i>
                        </div>
                        <div>
                            <span>Story</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="container3">
                <div class="md-form md-outline input-with-post-icon datepicker" inline="true">
                    <input placeholder="Select date" type="date" id="example" class="form-control">
                    <!-- <label for="example">Try me...</label> -->
                </div>
            </div>
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
    .btnn{
        width: 200px;
        height: 50px;
        border: none;
        border-radius: 10px;
    }
    .social-media{
        display: flex;
        margin-left: 30px;
        gap: 5px;
        height:60px;
        border-radius:10px;
    }
    .facebook ,.insta ,.youtube ,.twitter{
        font-size: 20px;
        padding: 15px;
        border-radius:8px 0px 0px 8px;
    }
    .bttn{
        width: 200x;
        height: 60px;
        border: black;
    }
    .container2{
        display: flex;
        gap: 50px;
    }
    .option{
        display: flex;
        /* display: inline; */
        gap: 5px;
        /* width: 230px; */
        /* height:60px; */
        border-radius:8px;
        align-items:center;
        justify-content: start;
    }
    .post , .story{
        display:flex;
        /* height: 60px; */
        font-weight: bold;
        /* border: 10px; */
        box-shadow: 20px;
        align-items:center;
        border-radius:8px 0px 0px 8px;
        /* justify-items: center; */
        justify-content: space-around;
        gap: 10px;
        padding: 10px 20px;
    }
    .post{
        /* width:90px; */
        background-color: #7E7E7E;
        color: white;
    }
    .story{
        /* width:90px; */
    }
    /* @import '~mdb-ui-kit/css/mdb.min.css'; */
    .cont{
        display: flex;
        justify-content: space-between;
    }
</style>