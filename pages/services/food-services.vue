<template>
    <div>
        <headerAndLog />
        <h1>halloo</h1>
        <footerLest />
    </div>
</template>

<style>
/* Start Global Rules */
:root {
    --main-color: #2196f3;
    --main-color-alt: #1787e0;
    --main-padding: 100px;
    --main-transition: 0.3s;
    --section-background: #ececec;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Work Sans', sans-serif;
}

a {
    text-decoration: none;
}

ul {
    list-style: none;
    padding: 0;
    margin: 0;
}

.container {
    padding-left: 15px;
    padding-right: 15px;
    margin-left: auto;
    margin-right: auto;
}

/* Small */
@media (min-width: 768px) {
    .container {
      width: 750px;
    }
}
  /* Medium */
@media (min-width: 992px) {
    .container {
      width: 970px;
    }
}
  /* Large */
@media (min-width: 1200px) {
    .container {
      width: 1170px;
    }
}
/* End Global Rules */
/* Start Main Titke */
.main-titl {
  border: 2px solid black;
  margin: 0 auto 80px;
  width: fit-content;
  padding: 15px 25px;
  position: relative;
  z-index: 10;
}
.main-titl:hover {
  color: white;
  border: 2px solid white;
  transition-delay: 1s;
}
.main-titl::before,
.main-titl::after{
  content: "";
  background-color: var(--main-color-alt);
  position: absolute;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  top: 50%;
  transform: translateY(-50%);
}
.main-titl::before{
  left: -30px;
}
.main-titl::after{
  right: -30px;
}

.main-titl:hover::before{
  z-index: -1;
  animation: left-down 1s linear forwards;
}
.main-titl:hover::after{
  z-index: -1;
  animation: right-down 1s linear forwards;
}
/* End Main Titke */
/* Start Animation */
@keyframes up-and-down {
  0%,
  100% {
    top: 0;
  }
  50% {
    top: 50px;
  }
}
@keyframes go-down {
  0%, 20%, 50%, 80%, 100% {
    transform: translate(0);
  }
  40%, 60% {
    transform: translateY(20px);
  }
}
@keyframes right-down {
  50% {
    right: 0;
    width: 12px;
    height: 12px;
  }
  100% {
    right: 0;
    width: 100%;
    height: 100%;
    border-radius: 0;
  }
}
@keyframes left-down {
  50% {
    left: 0;
    width: 12px;
    height: 12px;
  }
  100% {
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 0;
  }
}

@keyframes links-move {
  100% {
    transform: translateX(10px);
  }
}

@keyframes flashing {
  100% {
    width: 200%;
    height: 200%;
    opacity: 1;
  }
}
/* End Animation */
</style>