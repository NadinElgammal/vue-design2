<template>
  <section>
    <div class="container">
        <a href="#"><i class="fa-solid fa-chevron-right"></i></a>
        <a href="#"><i class="fa-solid fa-layer-group"></i></a>
        <a href="#"><i class="fa-solid fa-people-group"></i></a>
        <a href="#"><i class="fa-solid fa-inbox"></i></a>
        <a href="#"><i class="fa-solid fa-puzzle-piece"></i></a>
        <a href="#"><i class="fa-solid fa-wallet"></i></a>
        <a href=""><i class="fa-solid fa-chart-area"></i></a>
    </div>
  </section>
</template>

<script>
export default {
  name: "Sidebaar",
};
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css");
.container {
  background-color: #0164fb;
  height: 100%;
  width: 90px;
  display: flex;
  flex-direction: column;
  position: fixed;
  z-index: 2;
  top: 0;
  left: 0;
  overflow-x: hidden;
  padding-top: 20px;
}
i {
  font-size: 25px;
  color: #96befd;
  margin: 0px 0px 50px 15px;
}
</style>
