<template>
    <!-- Start Features -->
    <div class="features" id="features">
      <h2 class="main-titl">Features</h2>
      <div class="container">
        <div class="box quality">
          <div class="img-holder"><img src="../imgs/features-01.jpg" alt=""></div>
          <h2>Quality</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit harum hic veniam eligendi minima</p>
          <a href="#">More</a>
        </div>
        <div class="box time">
          <div class="img-holder"><img src="../imgs/features-02.jpg" alt=""></div>
          <h2>Time</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit harum hic veniam eligendi minima</p>
          <a href="#">More</a>
        </div>
        <div class="box passion">
          <div class="img-holder"><img src="../imgs/features-03.jpg" alt=""></div>
          <h2>Passion</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit harum hic veniam eligendi minima</p>
          <a href="#">More</a>
        </div>
      </div>
    </div>
    <!-- End Features -->
</template>

<style>
    /* Start Features */
.features {
  padding-top: var(--main-padding);
  padding-bottom: var(--main-padding);
  position: relative;
}

.features .container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 40px;
}

.features .box {
  text-align: center;
  border: 1px solid #ccc;
}

.features .box .img-holder{
  position: relative;
  overflow: hidden;
}

.features .box .img-holder::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgb(255 0 0 / 30%);
}
.features .quality .img-holder::before {
  background-color: rgb(244 64 54 / 60%);
}
.features .time .img-holder::before {
  background-color: rgb(0 150 136 / 60%);
}
.features .passion .img-holder::before {
  background-color: rgb(3 169 244 / 60%);
}


.features .box .img-holder::after {
  content: "";
  position: absolute;
  bottom: 0;
  right: 0;
  border-style: solid;
  border-width: 0px 0px 170px 500px;
  border-color: transparent transparent white transparent;
  transition: var(--main-transition);
}

.features .box .img-holder img{
  max-width: 100%;
}

.features .box:hover .img-holder::after {
  border-width: 100px 500px 170px 0px;
}

.features .box h2 {
  position: relative;
  margin: 0 auto 0;
  width: fit-content;
  font-size: 30px;
}

.features .box h2::after {
  content: "";
  position: absolute;
  bottom: -20px;
  left: 15px;
  height: 5px;
  background-color: red;
  width: calc(100% - 30px);
}
.features .quality h2::after{
  background-color: rgb(244 64 54 / 60%);
}
.features .time h2::after{
  background-color: rgb(0 150 136 / 60%);
}
.features .passion h2::after{
  background-color: rgb(3 169 244 / 60%);
}

.features .box p {
  padding: 20px 25px;
  line-height: 1.7;
  color: #777;
  font-size: 18px;
  margin: 30px 0;
}

.features .box a {
  display: block;
  border: 3px solid transparent;
  width: fit-content;
  margin: 0 auto 30px;
  font-weight: bold;
  font-size: 22px;
  padding: 10px 30px;
  border-radius: 6px;
  transition: var(--main-transition);
}
.features .quality a {
  border-color: rgb(244 64 54 );
  color: rgb(244 64 54);
  background: linear-gradient(to right, rgb(244 64 54) 50%, white 50%);
  background-size: 200% 100%;
  background-position: right bottom;
}
.features .time a {
  border-color: rgb(0 150 136);
  color: rgb(0 150 136);
  background: linear-gradient(to right, rgb(0 150 136) 50%, white 50%);
  background-size: 200% 100%;
  background-position: right bottom;
}
.features .passion a {
  border-color: rgb(3 169 244);
  color: rgb(3 169 244);
  background: linear-gradient(to right, rgb(3 169 244) 50%, white 50%);
  background-size: 200% 100%;
  background-position: right bottom;
}
.features .box:hover a {
  background-position: left bottom;
  color: white;
}

/* End Features */
</style>