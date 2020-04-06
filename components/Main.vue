<template>
<div class="main_section">
    <span class="main_bg"></span>
    <div class="links">
      <nuxt-link to="/intro" class="link">입관안내서</nuxt-link>
    </div>
  </div>
</template>
<style>
.main_logo {
  width: 100%;
  height: 100%;
  animation: 1s appear;
  margin: auto;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.main_section {
  position: relative;
  height: 100vh;
  width: 100vw;
  background-color: #000;
  padding-top: 20%;
}

.main_bg {
  display: block;
  background: no-repeat center url("../assets/imgs/main_logo.jpg");
  background-size: contain;
  min-height: 300px;
  background-color: #000;
}

.links {
  background-color: #000;
  padding-bottom: 60px;
}

.link {
  color: #fff;
  text-decoration: none;
  display: inline-block;
  padding: 10px 15px;
  font-size: 18px;
  border: 1px solid #fff;
  border-radius: 10px;

  -webkit-animation:blink 0.5s ease-in-out infinite alternate;
    -moz-animation:blink 0.5s ease-in-out infinite alternate;
    animation:blink 0.5s ease-in-out infinite alternate;
}

@-webkit-keyframes blink{
    0% {opacity:0.5;}
    100% {opacity:1;}
}
@-moz-keyframes blink{
    0% {opacity:0.5;}
    100% {opacity:1;}
}
@keyframes blink{
    0% {opacity:0.5;}
    100% {opacity:1;}
}

</style>
