<!-- HTML -->
<template>
    <!-- Start Header -->
    <header class="header-scrol">
        <div class="container">
            <a class="logo" href="http://localhost:3000/">Locaverse</a>
            <nav class="mein-nav">
                <ul class="mai-ul">
                    <li><a href="#articles">Services</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#">Other Links</a>
                         <!-- Start Megamenu -->
                      <div class="mega-menu">
                        <div class="image">
                          <img decoding="async" src="../imgs/megamenu.png" alt="">
                        </div>
                        <ul class="links">
                          <li>
                            <a href="services/food-services"><i class="far fa-user fa-fw"><font-awesome-icon :icon="['far','user']"/></i>Food Delivery</a>
                          </li>
                          <li>
                            <a href="services/taxi-services"><i class="far fa-building fa-fw"><font-awesome-icon :icon="['far','building']"/></i>Taxi Driver</a>
                          </li>
                          <li>
                            <a href="services/animals-services"><i class="far fa-check-circle fa-fw"><font-awesome-icon :icon="['far','check-circle']"/></i>Taking Care Of Animals</a>
                          </li>
                          <li>
                            <a href="services/fitness-services"><i class="far fa-clipboard fa-fw"><font-awesome-icon :icon="['far','clipboard']"/></i>Fitness Coach</a>
                          </li>
                        </ul>
                        <ul class="links">
                          <li>
                            <a href="services/computer-services"><i class="fas fa-server fa-fw"><font-awesome-icon :icon="['fas','server']"/></i>Computer Repair</a>
                          </li>
                          <li>
                            <a href="services/car-services"><i class="far fa-play-circle fa-fw"><font-awesome-icon :icon="['far','play-circle']"/></i>Car Repair</a>
                          </li>
                          <li>
                            <a href="services/house-services"><i class="far fa-chart-bar fa-fw"><font-awesome-icon :icon="['far','chart-bar']"/></i>House Cleaning</a>
                          </li>
                          <li>
                            <a href="services/child-services"><i class="fas fa-percent fa-fw"><font-awesome-icon :icon="['fas','percent']"/></i>Child Care</a>
                          </li>
                        </ul>
                      </div>
            <!-- End Megamenu -->
                    </li>
                </ul>
            </nav>
        </div>
    </header>
    <!-- End Header -->
</template>

<!-- CSS -->
<style>
/* Start Header */
.header-scrol {
    background-color: white;
    position: relative;
    -webkit-box-shadow: 0 0 10px #ddd;
    -moz-box-shadow: 0 0 10px #ddd;
    box-shadow: 0 0 10px #ddd;
    top: -7px;
}

.header-scrol .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    position: relative;
}

.header-scrol .container .logo {
  text-decoration: none;
  font-size: 30px;
  font-weight: bold;
  color: var(--main-color);
  display: flex;
  align-items: center;
  height: 72px;
}

.header-scrol .container .mein-nav {
    flex: 1;
}

@media (max-width:767px) {
     .header-scrol .container .logo {
        width: 100% !important;
        height: 50px !important;
        display: flex;
        justify-content: center;
    }
    .header-scrol .container .mein-nav .mai-ul {
        display: flex !important;
        justify-content: center !important;

    }
    .header-scrol .container .mein-nav .mai-ul > li > a {
        padding: 10px !important;
        font-size: 14px !important;
        height: 30px !important;
    } 
}

.header-scrol .container .mein-nav .mai-ul {
    display: flex;
    justify-content: flex-end;
    list-style: none;
}

.header-scrol .container .mein-nav .mai-ul > li > a {
    padding: 0 30px;
    font-size: 18px;
    text-decoration: none;
    color: black;
    list-style: none;
    display: flex;
    height: 72px;
    align-items: center;
    overflow: hidden;
    transition: var(--main-transition);
    position: relative;
}
.header-scrol .container .mein-nav .mai-ul > li > a::after{
    content: "";
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 4px;
    background-color: var(--main-color);
    transition: var(--main-transition);
}
.header-scrol .container .mein-nav .mai-ul > li > a:hover:after {
    left: 0;
}
.header-scrol .container .mein-nav .mai-ul > li > a:hover {
    background-color: #ccc;
    color: var(--main-color);
}
/* End Header */
/* Start Megamenu */
.header-scrol  .mai-ul > li:hover .mega-menu {
    opacity: 1;
    z-index: 100;
    top: 100%;
}

.header-scrol .mega-menu {
    position: absolute;
    width: 100%;
    left: 0;
    background-color: white;
    border-bottom: 3px solid var(--main-color);
    z-index: -1;
    display: flex;
    gap: 40px;
    top: calc(100% + 50px);
    opacity: 0;
    transition: top var(--main-transition), opacity var(--main-transition);
  }
  @media (max-width: 767px) {
    .header-scrol .mega-menu {
      flex-direction: column;
      gap: 0;
    }
  }
  
.header-scrol .mega-menu .image img {
    max-width: 100%;
  }
  @media (max-width: 991px) {
    .header-scrol .mega-menu .image {
      display: none;
    }
  }
  .header-scrol .mega-menu .links {
    min-width: 250px;
    flex: 1;
  }
  .header-scrol .mega-menu .links li {
    position: relative;
  }
  .header-scrol .mega-menu .links li:not(:last-child) {
    border-bottom: 1px solid #e9e6e6;
  }
  @media (max-width: 767px) {
    .header-scrol .mega-menu .links:first-of-type li:last-child {
      border-bottom: 1px solid #e9e6e6;
    }
  }
  .header-scrol .mega-menu .links li::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    width: 0;
    height: 100%;
    background-color: #fafafa;
    z-index: -1;
    transition: var(--main-transition);
  }
  .header-scrol .mega-menu .links li:hover::before {
    width: 100%;
  }
  .header-scrol .mega-menu .links li a {
    color: var(--main-color);
    padding: 15px;
    display: block;
    font-size: 18px;
    font-weight: bold;
  }
  .header-scrol .mega-menu .links li a i {
    margin-right: 10px;
  }
/* End Megamenu */
</style>