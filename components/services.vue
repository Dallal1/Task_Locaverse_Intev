<template>
    <!-- Start Articles -->
    <div class="articles" id="articles">
      <h2 class="main-titl">Services</h2>
      <div class="container">
        <a href="services/food-services">
          <div class="box">
            <img src="../imgs/Services-imag/food1.jpg" alt="">
            <div class="content">
              <h3>Food Delivery</h3>
              <p>Efficient delivery of delectable meals to your doorstep, guaranteed satisfaction.</p>
            </div>
            <div class="info">
              <a href="services/food-services">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/taxi-services">
          <div class="box">
            <img src="../imgs/Services-taxi/taxi1.jpg" alt="">
            <div class="content">
              <h3>Taxi Driver</h3>
              <p>Taxi services prioritize safety, reliability, cleanliness, professionalism, and efficiency.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/animals-services">
          <div class="box">
            <img src="../imgs/services-animals/animals1.jpg" alt="">
            <div class="content">
              <h3>Taking Care Of Animals</h3>
              <p>Ensuring the well-being and welfare of animals through dedicated care and compassion.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/fitness-services">
          <div class="box">
            <img src="../imgs/services-fitness/fitness1.jpg" alt="">
            <div class="content">
              <h3>Fitness Coach</h3>
              <p>A fitness coach provides tailored workouts, guidance, motivation, and support.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/computer-services">
          <div class="box">
            <img src="../imgs/services-computer/computer1.jpg" alt="">
            <div class="content">
              <h3>Computer Repair</h3>
              <p>Computer repair technician: Troubleshooting, fixing, upgrading, and optimizing computers.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/car-services">
          <div class="box">
            <img src="../imgs/services-car/car1.jpg" alt="">
            <div class="content">
              <h3>Car Repair</h3>
              <p>Auto repair service: Expertly diagnosing, fixing, and enhancing vehicle functionality.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/house-services">
          <div class="box">
            <img src="../imgs/services-house/house1.jpg" alt="">
            <div class="content">
              <h3>House Cleaning</h3>
              <p>House cleaning service: Thoroughly tidying, organizing, and sanitizing living spaces.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
        <a href="services/child-services">
          <div class="box">
            <img src="../imgs/services-child/child1.jpg" alt="">
            <div class="content">
              <h3>Child Care</h3>
              <p>Child care service: Caring, nurturing, and supervising children's well-being and development.</p>
            </div>
            <div class="info">
              <a href="">Read More</a>
              <i class="fas fa-long-arrow-alt-right">
                <font-awesome-icon :icon="['fas','long-arrow-alt-right']"/>
              </i>
            </div>
          </div>
        </a>
      </div>
    </div>
    <!-- End Articles -->
</template>


<style>
    /* Start Articles */
.articles {
  padding-top: var(--main-padding);
  padding-bottom: var(--main-padding);
  position: relative;
}

.articles .container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 40px;
  align-items: center;
}

.articles .box {
  box-shadow: 0 2px 15px rgb(0 0 0 / 10%);
  border-radius: 5px;
  overflow: hidden;
  margin: auto;
  transition: var(--main-transition);
}

.articles .box:hover {
  transform: translateY(-10px);
  box-shadow: 0 2px 15px rgb(0 0 0 / 20%);
}

.articles .box img {
   max-width: 100%; 
}

.articles .box .content {
  padding: 20px;
}

.articles .box .content h3 {
  margin: 0;
  color: #1c3540;
  font-size: 1.1rem;
  font-weight: bolder;
  word-break: break-word;
}

.articles .box .content p {
  color: #777;
  font-size: 15px;
  line-height: 1.6;
  margin-bottom: 0;
}

.articles .info {
  padding: 20px;
  border-top: 1px solid #ccc;
  display: flex;
  justify-content: space-between;
}

.articles .info a {
  color: var(--main-color);
  font-weight: bold;
}

.articles .info i {
  color: var(--main-color);
}

.articles .box:hover .info i {
  animation: links-move 1s linear infinite;
}

/* End Articles */
</style>