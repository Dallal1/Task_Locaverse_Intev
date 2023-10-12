<template>
    <!-- Start Gallery -->
    <div class="gallery" id="gallery">
      <h2 class="main-titl">Gallery</h2>
      <div class="container">
        <div class="box">
          <div class="image">
            <img src="../imgs/gallery-01.png" alt="">
          </div>
        </div>
        <div class="box">
          <div class="image">
            <img src="../imgs/gallery-02.png" alt="">
          </div>
        </div>
        <div class="box">
          <div class="image">
            <img src="../imgs/gallery-03.jpg" alt="">
          </div>
        </div>
        <div class="box">
          <div class="image">
            <img src="../imgs/gallery-04.png" alt="">
          </div>
        </div>
        <div class="box">
          <div class="image">
            <img src="../imgs/gallery-05.jpg" alt="">
          </div>
        </div>
        <div class="box">
          <div class="image">
            <img src="../imgs/gallery-06.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <!-- End Gallery -->
</template>

<style>
/* Start Gallery */
.gallery {
  padding-top: var(--main-padding);
  padding-bottom: var(--main-padding);
  background-color: var(--section-background);
}

.gallery .container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 40px;

}

.gallery .box {
  background-color: white;
  padding: 20px;
}

.gallery .box .image {
  position: relative;
  overflow: hidden;
}

.gallery .box .image::before {
  content: "";
  position: absolute;
  background-color: rgba(255, 255, 255, 0.3);
  width: 10px;
  height: 10px;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  opacity: 0;
  z-index: 2;
}
.gallery .box .image:hover:before {
  animation: flashing 0.7s;
}

.gallery .box .image img{
  max-width: 100%;
  transition: var(--main-transition);
}

.gallery .box .image:hover img {
  transform: rotate(6deg) scale(1.1);
}
/* End Gallery */
</style>