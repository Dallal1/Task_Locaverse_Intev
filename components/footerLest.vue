<template>
        <!-- Start Footer -->
        <div class="footer">
      <div class="container">
        <div class="box">
          <h3>Locaverse</h3>
          <ul class="social">
            <li>
              <a href="https://www.facebook.com/locaverse/" class="facebook">
                <i class="fab fa-facebook-f"><font-awesome-icon :icon="['fab','facebook-f']"/></i>
              </a>
            </li>
            <li>
              <a href="#" class="twitter">
                <i class="fab fa-twitter"><font-awesome-icon :icon="['fab','twitter']"/></i>
              </a>
            </li>
            <li>
              <a href="https://www.youtube.com/@Locaverse" class="youtube">
                <i class="fab fa-youtube"><font-awesome-icon :icon="['fab','youtube']"/></i>
              </a>
            </li>
          </ul>
          <p class="text">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Temporibus nulla rem, dignissimos iste aspernatur
          </p>
        </div>
        <div class="box">
          <ul class="links">
            <li><a href="#">Important Link 1</a></li>
            <li><a href="#">Important Link 2</a></li>
            <li><a href="#">Important Link 3</a></li>
            <li><a href="#">Important Link 4</a></li>
            <li><a href="#">Important Link 5</a></li>
          </ul>
        </div>
        <div class="box">
          <div class="line">
            <i class="fas fa-map-marker-alt fa-fw"><font-awesome-icon :icon="['fas','map-marker-alt']"/></i>
            <div class="info">THE ICON VIENNA Tower 24, 3rd Floor, BLRegister03, Wiedner Gürtel 13, 1100 Wien</div>
          </div>
          <div class="line">
            <i class="far fa-clock fa-fw"><font-awesome-icon :icon="['far','clock']"/></i>
            <div class="info">Business Hours: From 7:00 To 20:00</div>
          </div>
          <div class="line">
            <i class="fas fa-phone-volume fa-fw"><font-awesome-icon :icon="['fas','phone-volume']"/></i>
            <div class="info">
              <span>067761683900</span>
            </div>
          </div>
        </div>
        <div class="box footer-gallery">
          <img src="../imgs/gallery-01.png" alt="">
          <img src="../imgs/gallery-02.png" alt="">
          <img src="../imgs/gallery-03.jpg" alt="">
          <img src="../imgs/gallery-04.png" alt="">
          <img src="../imgs/gallery-05.jpg" alt="">
          <img src="../imgs/gallery-06.png" alt="">
        </div>
      </div>
      <p class="copyright">Made With &lt;3 By Dallal</p>
    </div>
    <!-- End Footer -->
</template>

<style>
/* Start Footer */
.footer {
  background-color: #191919;
  padding: 70px 0 0;
}
@media (max-width:767px) {
  .footer {
    text-align: center;
  }
}

.footer .container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 40px;
}

.footer .box h3 {
  color: white;
  font-size: 50px;
  margin: 0 0 20px;
}

.footer .box .social {
  display: flex;
  gap: 20px;
  justify-content: flex-start;
  align-items: center;
}

@media (max-width: 767px){ 
.footer .box .social {
    justify-content: center;
  }
}

.footer .box .social li {
  margin-right: 10px;
}

.footer .box .social li .facebook,
.footer .box .social li .twitter,
.footer .box .social li .youtube {
  background-color: #313131;
  color: #b9b9b9;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 50px;
  height: 50px;
  font-size: 20px;
  transition: var(--main-transition);
}

.footer .box .social li .facebook:hover {
  background-color: #1877f2;
}

.footer .box .social li .twitter:hover {
  background-color: #1da1f2;
}

.footer .box .social li .youtube:hover {
  background-color: #ff0000;
}

.footer .box .text {
  line-height: 2;
  color: #b9b9b9;
}

.footer .box .links li:not(:last-child){
  border-bottom: 1px solid #444;
}

.footer .box .links li {
  padding: 15px 0;
  transition: var(--main-transition);
}

.footer .box .links li:hover a {
  padding-left: 10px;
}

.footer .box .links li a{
  color: #b9b9b9;
  transition: var(--main-transition);
}

.footer .box .links li a::before {
  font-family: "Font Awesome 5 Free";
  content: "\F101";
  font-weight: 900;
  margin-right: 10px;
  color: var(--main-color);
}

.footer .box .line {
  display: flex;
  align-items: center;
  color: #b9b9b9;
  margin-bottom: 30px;
}

.footer .box .line .info {
  line-height: 1.7;
  flex: 1;
}

.footer .box .line i {
  font-size: 25px;
  color: var(--main-color);
  margin-right: 10px;
}

.footer .footer-gallery img {
  width: 72px;
  border: 3px solid white;
  margin: 2px;
}

.footer .copyright {
  padding: 25px 0;
  text-align: center;
  color: white;
  margin: 50px 0 0;
  border-top: 1px solid #444;
}

/* End Footer */
</style>