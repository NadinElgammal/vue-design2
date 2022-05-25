<template>
  <aside class="sidebar">
        <span class="menu"><i class="fa-solid fa-chevron-right icon"></i></span>
        <a href="#"><i class="fa-solid fa-layer-group "></i> <span id="text">New Tab</span></a>
        <a href="#"><i class="fa-solid fa-people-group"></i> <span id="text">Contact Us</span></a>
        <a href="#"><i class="fa-solid fa-inbox"></i><span id="text">Messages</span></a>
        <a href="#"><i class="fa-solid fa-puzzle-piece"></i><span id="text">Call Center</span></a>
        <a href="#"><i class="fa-solid fa-wallet"></i><span id="text">Wallet</span></a>
        <a href=""><i class="fa-solid fa-chart-area"></i><span id="text">Statistics</span></a>
  </aside>
</template>

<script>
export default {
  name: "Sidebaar",
  methods:{
  
  },
  mounted(){
    let menu = document.querySelector(".menu");
    menu.addEventListener("click" , () => {
      var sidebar = document.querySelector(".sidebar");
      var rightArrow = document.querySelector(".icon");
      var text = document.querySelectorAll("#text");
      if(sidebar.style.width === "200px"){
        sidebar.style.width = "90px"
        rightArrow.style.transform = "rotate(0deg)";
        text.forEach(element => {
          element.style.display = "none";
        });
      }
      else{
        sidebar.style.width = "200px"
        rightArrow.style.transform = "rotate(180deg)";
        text.forEach(element => {
          element.style.display = "block";
        });
      }
    })
  }
};
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css");
.sidebar {
  background-color: #0164fb;
  height: 100%;
  width: 90px;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;
  z-index: 15;
  top: 0;
  left: 0;
  overflow-x: hidden;
}

i {
  font-size: 25px;
  color: #96befd;
}

a{
  display: flex;
  width: 100%;
  text-align: center;
  justify-content: center;
  gap:10px;
  padding: 20px 0;
  transition: 0.5s;
  text-decoration: none;
}

a:hover{
  background-color:#0545a5 ;
  text-decoration: none;
}

.menu{
  display: block;
  width: 100%;
  text-align: center;
  padding: 20px 0;
  transition: 0.5s;
  cursor: pointer;
}
.menu:hover{
  background-color:#0545a5 ;
}

#text{
  /* visibility: hidden; */
  display: none;
  color: white;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

</style>
