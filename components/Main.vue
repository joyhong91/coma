<template>
  <img src="~/assets/imgs/main_logo.jpg" class="main_logo"/>
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
</style>
