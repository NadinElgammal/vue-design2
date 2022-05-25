<template>
    <div class="container">
        <div class="row">
          <div class="col-xl-2 col-lg-4 col-md-4 col-sm-6 col-12">
            <div class="card" >
              <div class="icon-part">
                <i class="fa-solid fa-chart-line" style="color:#0164fb;"></i> <br>
              </div>
              <div class="text-part">
                <h4>
                  3,56% 
                </h4>
                <span>
                  engagment 
                </span>
                <br> <br>
              </div>
            </div>
          </div>
          <div class="col-xl-2 col-lg-4 col-md-4 col-sm-6 col-12">
            <div class="card" >
              <div class="icon-part">
                  <i class="fa-solid fa-people-group" style="color:gray"></i>
              </div>
              <div class="text-part">
                <h4>
                  1 001 856
                </h4>
                <span>
                  reach
                </span>
                <br> <br>
              </div>
            </div>
          </div>
          <div class="col-xl-2 col-lg-4 col-md-4 col-sm-6 col-12">
            <div class="card" >
              <div class="icon-part">
                <i class="fa-solid fa-eye" style="color:gray"></i>
              </div>
              <div class="text-part">
                <h4>
                  1 556 000
                </h4>
                <span>
                  impressions 
                </span>
                <br> <br>
              </div>
            </div>
          </div>
          <div class="col-xl-2 col-lg-4 col-md-4 col-sm-6 col-12">
            <div class="card" >
              <div class="icon-part">
                <i class="fa-solid fa-heart" style="color:#D97485"></i><span style="font-size:12px; color:black; margin:5px">15%</span>
              </div>
              <div class="text-part">
                <h4>
                  156 785
                </h4>
                <span>
                  likes 
                </span>
                <br> <br>
              </div>
            </div>
          </div>
          <div class="col-xl-2 col-lg-4 col-md-4 col-sm-6 col-12">
            <div class="card" >
              <div class="icon-part">
                <i class="fa-solid fa-comment" style="color:#9FC883"></i><span style="font-size:12px; color:black; margin:5px">10%</span>
              </div>
              <div class="text-part">
                <h4>
                  56 000 
                </h4>
                <span>
                  comments 
                </span>
                <br> <br>
              </div>
            </div>
          </div>
          <div class="col-xl-2 col-lg-4 col-md-4 col-sm-6 col-12">
            <div class="card" >
              <div class="icon-part">
                <i class="fa-solid fa-download" style="color:#D8BD85"></i><span style="font-size:12px; color:black; margin:5px">0.5%</span>
              </div>
              <div class="text-part">
                <h4>
                  1200 
                </h4>
                <span>
                  saved 
                </span>
                <br> <br>
              </div>
            </div>
            <br><br>
          </div>
        </div>
      </div>
</template>

<script>
export default {
  name:"Statistics",
}
</script>

<style scoped>
.card{
  display: flex;
  align-items: center;
  font-size: 13px;
  background-color: #F5F6F9;
  border-radius: 10px;
}
.icon-part{
  font-size: 19px;
  color: #0164fb;
  padding: 5px;
}
h4{
  font-weight: bold;
}
.text-part{
  display: flex;
  flex-direction: column;
  align-content: center;
  align-items: center;
}
</style>

