<template>
     <!-- Start Landing -->
     <div class="landing">
      <div class="container">
        <div class="text">
          <h2>Welcome, To Locaverse World</h2>
          <p>We offer eight core services. Here, all of Locaverse's services are at your disposal</p>
        </div>
        <div class="image">
          <img src="../static/landing-image.png" alt="">
        </div>
      </div>
      <a href="#articles" class="go-down">
        <i class="fas fa-angle-double-down fa-2x">
          <font-awesome-icon :icon="['fas','angle-double-down']"/>
        </i>
      </a>
    </div>
    <!-- End Landing -->
</template>

<style>
/* Start Landing */
.landing {
 position: relative;
}
.landing::before {
  content: "";
  position: absolute;
  background-color: #ccc;
  left: 0;
  top: -40px;
  width: 100%;
  height: 100%;
  z-index: -1;
  transform: skewY(-9deg);
  transform-origin: top left;
 }

.landing .container {
  height: calc(100vh - 72px);
  display: flex;
  align-items: center;
  padding-bottom: 10px;
}

.landing .text {
  flex: 1;
}

@media (max-width: 767px) {
  .landing .text  {
    text-align: center;
  }
} 

.landing .text h2 {
  margin: 0;
  letter-spacing: -1px;
  font-size: 40px;
}
@media (max-width: 767px) {
  .landing .text h2  {
    font-size: 30px;
  }
} 
.landing .text p {
  font-size: 20px;
  line-height: 1.5;
  color: #666;
}
@media (max-width: 767px) {
  .landing .text p  {
    font-size: 15px;
  }
} 
.landing .image img {
  width: 600px;
  position: relative;
  animation: up-and-down 3s linear infinite;
}
@media (max-width: 991px) {
  .landing .image {
    display: none;
  }
}

.landing .go-down {
  position: absolute;
  color: var(--main-color);
  bottom: 30px;
  left: 50%;
  transform: translateY(-50%);
  transition: var(--main-transition);
}

.landing .go-down:hover {
  color: var(--main-color-alt);
}

.landing .go-down i {
  animation: go-down 1.5s linear infinite;
}
/* End Landing */
</style>