<template>
  <div class="container">
    <div class="row">
      <div class="col-xl-3 col-lg-3 col-md-4 col-sm-6 col-12" v-for="Post in Posts" :key="Post.id">
        <div class="card">
          <div class="img-part">
            <img :src="Post.image">
          </div>
          <div class="card-cont1">
            <div class="text-part">
            <span class="name">
              {{ Post.name }}
            </span>
            <br />
            <span class="desc">
              {{ Post.desc }}
            </span>
            </div>
            <div>
              <span class="price"> {{ Post.GBP }} GBP </span>
              <br>
              <span class="date"> {{Post.date}} </span>
            </div>
          </div>
          <div class="stats">
            <div class="reach">
              <span style="font-weight:bold; font-size:15px">{{Post.reach}}</span>
              <span>reach</span>
            </div>
            <span> | </span>
            <div class="imp">
              <span style="font-weight:bold;">{{Post.impressions}}</span>
              <span>impressions</span>
            </div>
          </div>
          <div class="circle1">
            <img :src="Post.image" class="c1">
          </div>
          <div class="circle2">
            <i class="fa-brands fa-instagram" style="font-size:20px; padding:7px"></i>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"Cards",
  data() {
    return {
      Posts: [
        {
          id: 1,
          name: "Lorem ipsum dolor",
          desc: "ipsum dolor",
          GBP: 405,
          date: "Nov 15,2020",
          reach: "1 100 576",
          impressions: "1 675 576",
          image : "https://i.pinimg.com/736x/f9/33/20/f933203940a396ae98bdab3bf7fa49f7.jpg"       
        },
        {
          id: 2,
          name: "Lorem ipsum dolor",
          desc: "ipsum dolor",
          GBP: 246,
          date: "Nov 15,2020",
          reach: "1 100 576",
          impressions: "1 675 576",
          image:"https://i.pinimg.com/550x/cd/30/67/cd3067cd04790531cdb383a44a815e49.jpg"
        },
        {
          id: 3,
          name: "Lorem ipsum dolor",
          desc: "ipsum dolor",
          GBP: 454,
          date: "Nov 15,2020",
          reach: "1 100 576",
          impressions: "1 675 576",
          image:"https://i.pinimg.com/474x/48/6c/a0/486ca00640b169300b48e9ceacd8e401.jpg"
        },
        {
          id: 4,
          name: "Lorem ipsum dolor",
          desc: "ipsum dolor",
          GBP: 543,
          date: "Nov 15,2020",
          reach: "1 100 576",
          impressions: "1 675 576",
          image:"https://i.pinimg.com/originals/0e/6c/3b/0e6c3b0bff65dd7882551446c9301137.jpg"
        },
        {
          id: 5,
          name: "Lorem ipsum dolor",
          desc: "ipsum dolor",
          GBP: 165,
          date: "Nov 15,2020",
          reach: "1 100 576",
          impressions: "1 675 576",
          image:"https://i.pinimg.com/originals/a7/80/80/a7808059330f062de8a90e844d0558d1.png"
        },
      ],
    };
  },
}
</script>


<style>
.card {
    width: 100%;
    /* box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25); */
    overflow: hidden;
    margin-bottom: 20px;
    transition: 0.5s;
    border-radius: 5  px !important;
    display: flex;
    align-content: center;
    transition: 0.3s;
}

.img-part {
    position: relative;
    width: 100%;
    height: 100%;
    /* clip-path: circle(210px at center 0); */
    /* border-radius: 0 0 50% 50% ; */
    /* transform: scaleX(2); */
    overflow: hidden;
}

img{
    width: 100%;
    object-fit: cover;
}

.reacts{
    position:absolute;
    top: 20px;
    right: 10px;
}

.text-part{
  margin: 18px;
}

.date{
  font-size: 12px;
}
.name{
    font-size : 14px;
    font-weight : bold;
}
.desc{
  font-size: 12px;
    color:#1B53EC;
}
.price{
    font-weight: bold;
    font-size: 13.5px;
}

.card:hover{
    transform:scale(1.04);
    z-index:2;
    /* transition: 0.3s; */
}
.card-cont1{
  display: flex;
  justify-content: space-around;
  align-items: center;
  gap:5px
}

.stats{
  background-color: #e4ebfa;
  width: 75%;
  border-radius: 10px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 14px;
  margin: 0 20px 10px 30px; 
}

.reach , .imp{
  display: flex;
  flex-direction: column;
  align-content: center;
}

.circle2{
  border: 3px solid #ffffff;  
  border-radius: 50%;
  width: 40px;
  height: 40px;
  background:linear-gradient(100deg,#E4914C,#C74D7B) ;
  color:#FFFFFF;
  left: 8px;
  bottom: 120px;
}

.circle1{
  
  left: 30px;
  bottom: 120px;
  z-index: 2;
}
.c1{
  border: 3px solid #ffffff;
  border-radius: 50%;
  width: 40px;
  height: 40px;
}

.circle1 , .circle2{
  position: absolute;

}

</style>