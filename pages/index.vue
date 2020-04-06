<template>
  <div class="container">
    <div>
      <h1 class="title">
      </h1>
      <h2 class="subtitle">
      </h2>
      <Main/>
      
      
      
    </div>
  </div>
</template>

<script>
import Main from '~/components/Main.vue'

export default {
  components: {
    Main
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #000;
}

.title {
}

.subtitle {
}


</style>
