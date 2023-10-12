<template>
    <!-- Start Testimonials -->
    <div class="Testimonials" id="Testimonials">
      <h2 class="main-titl">Testimonials</h2>
      <div class="container">
        <div class="box">
          <img src="../imgs/avatar-01.png" alt="">
          <h3>Mohamed Farag</h3>
          <span class="title">Full Stack Developer</span>
          <div class="rate">
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="far fa-star"></i>
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores et reiciendis voluptatum, amet est natus
            quaerat ducimus
          </p>
        </div>
        <div class="box">
          <img src="../imgs/avatar-02.png" alt="">
          <h3>Mohamed Ibrahim</h3>
          <span class="title">Full Stack Developer</span>
          <div class="rate">
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="far fa-star"></i>
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores et reiciendis voluptatum, amet est natus
            quaerat ducimus
          </p>
        </div>
        <div class="box">
          <img src="../imgs/avatar-03.png" alt="">
          <h3>Shady Nabil</h3>
          <span class="title">Full Stack Developer</span>
          <div class="rate">
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="far fa-star"></i>
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores et reiciendis voluptatum, amet est natus
            quaerat ducimus
          </p>
        </div>
        <div class="box">
          <img src="../imgs/avatar-04.png" alt="">
          <h3>Amr Hendawy</h3>
          <span class="title">Full Stack Developer</span>
          <div class="rate">
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores et reiciendis voluptatum, amet est natus
            quaerat ducimus
          </p>
        </div>
        <div class="box">
          <img src="../imgs/avatar-05.png" alt="">
          <h3>Sherief Ashraf</h3>
          <span class="title">Full Stack Developer</span>
          <div class="rate">
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="far fa-star"></i>
            <i class="far fa-star"></i>
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores et reiciendis voluptatum, amet est natus
            quaerat ducimus
          </p>
        </div>
        <div class="box">
          <img src="../imgs/avatar-06.png" alt="">
          <h3>Osama Mohamed</h3>
          <span class="title">Full Stack Developer</span>
          <div class="rate">
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="filled fas fa-star"></i>
            <i class="far fa-star"></i>
            <i class="far fa-star"></i>
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores et reiciendis voluptatum, amet est natus
            quaerat ducimus
          </p>
        </div>
      </div>
    </div>
    <!-- End Testimonials -->
</template>

<style>
/* Start Testimonials */
.Testimonials {
  padding-top: var(--main-padding);
  padding-bottom: var(--main-padding);
  background-color: var(--section-background);
}

.Testimonials .container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 40px;
}

.Testimonials .box {
  background-color: white;
  box-shadow: 0 2px 15px rgb(0 0 0 / 10%);
  border-radius: 5px;
  padding: 20px;
  position: relative;
}

.Testimonials .box img {
  position: absolute;
  width: 80px;
  right: -15px;
  top: -50px;
  border-radius: 50%;
  border: 10px solid #ececec;
}

.Testimonials .box h3 {
  margin: 0 0 10px;
  font-weight: 600;
  font-size: 20px;
}

.Testimonials .box .title {
  margin: 0 0 10px;
  display: block;
  color: #777;
}

.Testimonials .box .rate .filled {
  color: #ffc107;
}

.Testimonials .box p {
  line-height: 1.5;
  color: #777;
  margin-top: 10px;
  margin-bottom: 0;
}
/* End Testimonials */
</style>