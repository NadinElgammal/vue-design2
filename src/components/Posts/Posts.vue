<template>
<section>
  <div class="container1">
    <div>
      <div class="form">
        <i class="fa fa-search"></i>
        <input
          type="text"
          class="form-control form-input"
          placeholder="Search"
        />
      </div>
    </div>
    <div class="select">
      <span for="exampleFormControlSelect1" style="color: #9ca3af">Sort by:</span>
      <div>
        <select class="form-control selector">
          <option>Publication date</option>
          <option>2</option>
          <option>3</option>
          <option>4</option>
          <option>5</option>
        </select>
      </div>
      <i class="fa-solid fa-arrow-down-wide-short"></i>
      <span> | </span>
      <i class="fa-solid fa-plus"></i>
      <br />
      <br />
    </div>
  </div>
  <br> <br>
  <Cards />
</section>
</template>

<script>
import Cards from "./Cards.vue"
export default {
  name: "Posts",
  components:{
    Cards
  }
};
</script>

<style scoped>
.container1 {
  display: flex;
  justify-content: space-around;
  gap: 40%;
  align-items: center;
}

.select {
  display: flex;
  gap: 20px;
  align-items: center;
}

.selector {
  width: 200px;
}

.form {
  position: relative;
}

.form .fa-search {
  position: absolute;
  top: 20px;
  left: 20px;
  color: #9ca3af;
}

.form span {
  position: absolute;
  right: 17px;
  top: 13px;
  padding: 2px;
  border-left: 1px solid #d1d5db;
}

.left-pan {
  padding-left: 7px;
}

.left-pan i {
  padding-left: 10px;
}

.form-input {
  height: 55px;
  text-indent: 33px;
  border-radius: 7px;
  width: 300px;
}
</style>